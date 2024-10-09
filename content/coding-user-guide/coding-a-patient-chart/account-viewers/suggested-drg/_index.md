+++
title = 'Suggested DRG Viewer'
weight = 80
+++

Fusion CAC suggests a DRG on inpatient charts. This Suggested DRG is computed by the system within a
set interval (typically every six hours of the patient’s admission provided there is enough documentation
to suggest codes used to compute a DRG).

The Suggested DRG is then re-calculated every six hours until discharge or a CDI Specialist or Coder
computes a DRG. At that time the Suggested DRG is discontinued. The Suggested DRG along with other
data elements are not commonly used within Fusion CAC, rather this data is sent outbound to be used
by other healthcare professionals ,such as physicians and case managers, to predict the number of days
that the insurance (payor) will pay for the patient to stay within the hospital based upon the current
diagnosis of the patient. The common data element used by case management and physicians is called
the GMLOS (Geometric Means Length of Stay).

## How does suggested DRG work?

The suggested DRG module leverages the codes that are suggested by the FAE engine. The FAE engine
collects all codes suggested along with the section header that it was extracted from. The diagnosis
codes are then compared against a configuration file called “Invalid Headers”. If the diagnosis came
from a section header within this file it is discarded from consideration for the principal diagnosis. The
principal diagnosis code commonly is the driver of the DRG category; thus, the section of what diagnosis
is named principal is crucial in the success of the Suggested DRG. Once the codes have been picked
through for candidates, the codes are then passed through a modeling system to select the principal
diagnosis based upon historical data that the model has been trained upon.

## Why do we discard diagnosis from being candidates for a principal diagnosis?

A patient’s chart contains a lot of information including historical information that is relevant for the
patient’s chart, but should not be considered as a principal diagnosis. The principal diagnosis can be
defined as primary diagnosis to which the majority of the resources were applied or the main reason the
patient was admitted. The “invalid headers” that are thrown out include medical history, problem list,
social history, and family history, among others.

## How is Suggested DRG displayed with Fusion CAC?

It is displayed within a viewer called Suggested DRG. This is housed under the navigation tree and
displayed for users to see the timeline of the suggested DRG and how it evolved overtime. Below is a
screenshot of what the suggested DRG viewer looks like within the navigation tree. By clicking on the
blue header the tree will expand and show the coder along with the principal diagnosis that was
selected.

![Alternative Working DRG](image-180.jpg)