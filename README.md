## A Cross-Task Visuo-Tactile Representation Using Point Clouds

This page is currently including the abstract of the paper (under review), the outline of the project, and supplementary analyses.

## Table of Contents

1. [Abstract](#abstract)
2. [Outline](#outline)
3. [Supplementary](#supplementary)
4. [References](#references)

---

## Abstract

The combination of visual and tactile cues has proved to be effective for object recognition as well as grasping and manipulation tasks. Nevertheless, the two modalities are not trivial to combine since tactile and visual data carry distinct information and may be structurally different. Researchers have addressed this problem by proposing approaches that either do not consider mechanical properties conveyed by tactile sensors or cannot be deployed directly for diverse tasks. In this paper, we propose a cross-task visuo-tactile representation that encodes both the geometrical and mechanical properties of objects in a point cloud data structure. By physically exploring different areas of a given item, we collect tactile information to estimate the local compliance of the surface, encoding it as the color information of the point cloud in the probed areas. Then, this color information is extended to the entire object assuming that neighboring points share the same mechanical properties. We apply the proposed point cloud to a set of 6 real-world objects showing that it  can be effectively used to encode the shape of the objects along with their information on the local compliance. Further, we show that the augmented point cloud can be used for different tasks by exploiting this in three robotic tasks - a visuo-tactile object classification problem, a path following and a reaching in clutter tasks.

---

## Outline

In the manuscript, we present a cross-task representation that leverages the point cloud (PC) data structure to encode visuo-tactile cues. In particular, a PC acquired with RGB-D cameras is used to represent the geometry of the objects, while tactile sensing ([Cyskin](#https://www.cyskin.com/)) is used to augment it  with physical information embedded in the color assigned to the cloud. Specifically, we use this representation to encode the compliance distribution across the whole object’s surface. We showed how the proposed representation can be used to enhance robot abilities across different tasks, such as object classification, by using directly a state-of-the-art classifier like [PointNet](#https://github.com/charlesq34/pointnet), and control tasks including path following, and reaching in clutter.

This work was supported by he SESTOSENSO (HORIZON EUROPE Research and Innovation Actions under GA number 101070310).

---

# Supplementary
## Gaussian Process based representation 

In this section, we will discuss the Gaussian Process (GP) based representation of the data. 
As a matter of fact, GP-based representation are widely used and could serve as a way of combining mechanical and visual properties. For a formal introduction to GP, we refer the reader to [[1](#1)].


---

## References

1. C. Williams and C. Rasmussen, “Gaussian processes for regression,” Advances in neural information processing systems, vol. 8, 1995.