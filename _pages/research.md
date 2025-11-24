---
layout: page
title: Research
permalink: /research/
author_profile: true
---


{% include base_path %}

![Alt text](/images/Di-research-0.jpg)

<div style="margin: 100px;" markdown="1">

<p>
Nature showcases small organisms with remarkable individual locomotion capabilities and collective behaviors — from hummingbirds displaying exceptional agility and precise hovering, to schools of fish navigating thousands of miles in coordinated, adaptive group patterns.

These collectives demonstrate an incredible level of  <strong>self-organization</strong>, where large numbers of relatively simple agents rely on local interactions to produce complex global behaviors. As a result, the system as a whole becomes greater than the sum of its parts. What makes these systems so fascinating to scientists and engineers is that, despite each individual having limited capabilities, the collective achieves a remarkable degree of autonomy and complexity.
</p>


<p>
My research draws inspiration from biological systems and aims to develop <strong>artificial collectives</strong> of our own. I focus on creating cost-effective, small-scale robots that can form robotic fleets mimicking biological collectives in several highly desirable ways:

<ul>
    <li>Exhibiting complex behavior across large scales despite each individual being simple and has severely limited perception (scalable);</li>
    <li>Achieving decentralized coordination with high robustness to individual failures (robust);</li>
    <li>Leveraging collaborative action and sensing to cope with a broad spectrum of different enviorment and tasks (flexible).</li>
</ul>
My research is organized around the following three aims to advance this vision.
</p>

# Research Areas

## Decentralized Coordination Principles for Swarms
<!-- ![Alt text](/images/Di_research_summary.png) -->
<div style="display: flex; align-items: flex-start; gap: 20px; margin: 20px 0;">
    <div style="flex: 2;">
        <p>
        Fish schools is one of the well-known examples of collective behavior: thousands of fish migrate together, form dyanmics formation to navigate across cluttered environment, and form dynamic shapes like bait balls to evade predators. Underwater robot collectives may achieve similar benefits using formation control in future applications, e.g. efficient spatial sampling for environmental monitoring. 
        </p>
        <p>        
Using <strong>BlueSwarm</strong>, an underwater swarm platform consisting of 10 Bluebots, we have demonstrated multiple robots navigate in a variety of formations, including following behind or alongside each other, moving above and below, and maintaining diamond-shaped configurations, all based on noisy local visual interactions. This work represents the first experimental realization of entirely vision-based 3D formation control in miniature underwater robots, employing a behavior-based leader-follower strategy. The successful implementation with physical robots not only creates new opportunities for studying fish schooling using
robotic platforms but also advances the development of
implicit coordination algorithms for dynamic formation
control, where agents must continuously adapt to changing
positions and motions, a significantly greater challenge than
maintaining static configurations.
        </p>
        <p>
        Future work will focus on advancing underwater perception through natural-light vision systems and data-driven approaches to handle challenging optical conditions and complex enviornments. These developments will support more scalable and sophisticated swarm behaviors, bringing us closer to using robot collectives to study and interact with natural biological systems.
        </p>
    </div>
    <div style="flex: 1; text-align: center;">
        <video width="100%" autoplay loop muted playsinline>
                    <source src="/images/diamond_x8.mp4" type="video/mp4">
                    Your browser does not support the video tag.
                </video>
        <img src="/images/Di-research-1.png" alt="Research Image" style="width: 100%; max-width: 500px;">
        <br>
        <!-- <video width="100%" controls>
            <source src="/videos/Di-research-video.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video> -->
    </div>
</div>


## Perception and Control Strategies for Small-Scale, Resource-Constrained Robots

<!-- ![Alt text](/images/Di_research_summary.png) -->
<div style="display: flex; align-items: flex-start; gap: 20px; margin: 20px 0;">
    <div style="flex: 2;">
        <p>
        In idealized models and control laws, robots are often assumed to have extensive knowledge of the environment, precise awareness of their own states, and abundant computational resources. These assumptions rarely hold for small robots with limited resources. However, enabling such robots to make local decisions without relying on global information or centralized computation is critical, particularly for swarm deployment in complex or unstructured environments.
        </p>
        <p>        
        We have developed several fish-inspired platforms to explore embodied intelligence and fully autonomous decision-making. In the underwater domain, robots face severe constraints: sensing is often noisy and can be subject to occlusion, actuation is hindered by fluid, and communication is hard due to the absence of RF signals, making the underwater environment a natural testbed for decentralized strategies. A central effort of my work was <strong>Bluebots</strong>, a fish-inspired underwater robot with 3D motion maneuverability and 3D visual perception. We are developing lightweight models for robust and decentralized perception and control on small, resource-constrained robots, to bring robots closer to
real-world deployment.
        </p>
    </div>
    <div style="flex: 1; text-align: center;">
        <img src="/images/Di-research-2.1.jpg" alt="Research Image" style="width: 100%; max-width: 500px;">
        <video width="100%" autoplay loop muted playsinline>
                    <source src="/images/Di-research video dualcamera mangrove low res.mp4" type="video/mp4">
                    Your browser does not support the video tag.
                </video>
        <img src="/images/Di-research-2.2.png.jpg" alt="Research Image" style="width: 100%; max-width: 500px;">
        <br>
        <!-- <video width="100%" controls>
            <source src="/videos/Di-research-video.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video> -->
    </div>
</div>




## Innovative Actuation, Sensing, and Power Solutions for Small-scale Robots

Currently, most small-scale robots still lack the payload capacity and on-board resources for full autonomy. Developing strong actuators and compact power supplies is therefore essential for enabling truly autonomous small robots.

To enable a small robot with large payload, I developed a miniaturized electrostatic actuator with a high energy density. Inspired by skeletal muscles, the 3D polymer interdigitated pillar electrostatic actuator (PIPE) mimics the honeycomb structure of muscle fibers. By arranging two chips with interleaving pillar arrays, PIPE actuators increase the overlapping surface area in 3D, thus amplifying the output density of force and energy. My analytical model predicts that further miniaturization (reducing pillar gaps to 10 µm or smaller) will yield force densities 5–10× higher than biological muscle. To address the high voltages required by small-scale electric field actuators, I also developed a mm-scale kilovolt generator using pyroelectricity (LiNbO3) that demonstrate a 1–3 kV generation in a volume of 0.25 cm³ . The device can be solar powered and operated in a distributed architecture for local kV powering of multi-actuator systems. Such designs allow robots to harvest widely available thermal energy, reducing reliance on tethered power or frequent recharging. Future research will build on these foundations to develop hardware specifically optimized for small robots.



</div>

---
