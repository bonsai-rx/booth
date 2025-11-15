# Real-Time Place Preference Example

An example of a real-time place preference (RT-PP) task in [Bonsai](https://bonsai-rx.org/). 

This example demonstrates how to use the [Harp Hobgoblin](https://harp-tech.org/tutorials/hobgoblin-setup.html) for basic close-loop control and how to build a simple experimental graphical user interface using the [Bonsai.GUI](https://bonsai-rx.org/gui/) package.

## How to use

This example assumes that there are two regions of interest, one on the left and one on the right, and that a segmented object moving into the right region will trigger an optogenetic pulsetrain stimulation.

1) Draw two regions of interest (one on the left and one on the right) using the `Regions` property editor in the graphical interface.
2) Adjust the detection parameters to isolate your object.
3) (Optional) To simulate a pulsetrain, connect a LED wired up with a 100 Ω resistor to `GP15` on the `Hobgoblin`, and click on the `Enable Optogenetic Stimulation` button.

This example will also work if you do not have a `Hobgoblin` on hand, in which case the pulsetrain controls will have no effect.