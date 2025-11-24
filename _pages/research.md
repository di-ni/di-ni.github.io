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

## Coordination Principles for Swarms
<!-- ![Alt text](/images/Di_research_summary.png) -->
<div style="display: flex; align-items: flex-start; gap: 20px; margin: 20px 0;">
    <div style="flex: 2;">
        <p>
        Self-organizing collectives in the natural world have long inspired swarm robotics, where large numbers of relatively simple agents use local interactions to produce impressive global behaviors. For small robots, while each individual may be limited in payload, sensing, and computational capacity, collectively they have the potential to achieve great complexity. Discovering the coordination principles can enable swarms to achieve tasks that are impossible for a single robot, such as robust exploration, distributed sensing, and energy-efficient navigation.
        <!-- The schooling behavior of fish is hypothesized to confer many survival benefits, including foraging success, safety from predators, and energy savings through hydrodynamic interactions when swimming in formation. Underwater robot collectives may achieve similar benefits using formation control in future applications, e.g. efficient spatial sampling for environmental monitoring. Although many theoretical algorithms exist for multi-robot formation control, few have been tested in the underwater domain due to fundamental challenges in underwater communication.  -->
        </p>
        <p>
        Fish schools is one of the well-known examples of collective behavior: thousands of fish migrate together, form dyanmics formation to navigate across cluttered environment, and form dynamic shapes like bait balls to evade predators. Underwater robot collectives may achieve similar benefits using formation control in future applications, e.g. efficient spatial sampling for environmental monitoring. 
        </p>
        <p>        
Using <strong>BlueSwarm</strong>, an underwater swarm platform consisting of 10 Bluebots, we have demonstrated that <strong>{multiple robots navigate in a variety of formations</strong>, including following behind or alongside each other, moving above and below, and maintaining diamond-shaped configurations, all based on noisy local visual interactions. This work represents the first experimental realization of entirely vision-based 3D formation control in miniature underwater robots, employing a behavior-based leader-follower strategy. The successful implementation with physical robots not only creates new opportunities for studying fish schooling using
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
        <img src="/images/Di-research-1.jpg" alt="Research Image" style="width: 100%; max-width: 500px;">
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
        We have developed several fish-inspired platforms to explore embodied intelligence and fully autonomous decision-making. In the underwater domain, robots face severe constraints: sensing is often noisy and can be subject to occlusion, actuation is hindered by fluid, and communication is hard due to the absence of RF signals, making the underwater environment a natural testbed for decentralized strategies. A central effort of my work was
\underline{Bluebots}, a fish-inspired underwater robot with \underline{3D motion maneuverability and 3D visual perception}. 
Using fast onboard image processing, a Bluebot can perform real-time 3D pose and heading estimation entirely from cameras and LEDs, creating a minimalist yet versatile visual system. It uses a reactive controller and achieves rates up to 5 Hz on a Raspberry Pi Zero. Through purely visual observation of the environment and neighboring robots, we showed that the Bluebot can make decisions fully onboard without relying on global positioning or centralized control.
        </p>
        <p>
        Future research will build on this groundwork to bring robots closer to real-world deployment.
With the rapid progress of AI, powerful models have been developed for tasks such as object detection and depth estimation. However, underwater perception remains very challenging due to low visibility, dynamic lighting, and limited data availability. By tailoring AI models to these conditions and leveraging advances in compact computing hardware, robots can transition from laboratory testing to field operation. My ongoing work uses DepthAnything to enable robots to perform depth estimation with monocular cameras. Building on this foundation, I will continue to develop lightweight models for robust and decentralized perception and control on small, resource-constrained robots.
This effort involves both algorithmic-level optimization, such as model compression and domain-specific training for underwater vision, as well as system-level integration with limited onboard computation, sensing, and control. 
        </p>
    </div>
    <div style="flex: 1; text-align: center;">
        <video width="100%" autoplay loop muted playsinline>
                    <source src="images/Di-research video dualcamera mangrove low res.mp4" type="video/mp4">
                    Your browser does not support the video tag.
                </video>
        <img src="/images/Di-research-2.jpg" alt="Research Image" style="width: 100%; max-width: 500px;">
        <br>
        <!-- <video width="100%" controls>
            <source src="/videos/Di-research-video.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video> -->
    </div>
</div>




## Actuation and Power in mm-cm Scale

(Coming soon) Despite significant progress in small-sized robotic
systems over the past two decades, most platforms
lack sufficient payload capacity for onboard power
due to size constraints. Developing strong actuators
and compact power supplies is thus crucial for realizing
full autonomous operation in small robots.
 <!-- While
individual miniature robots have limited payload and
computing capacity, exploring swarm strategies can
potentially overcome these limitations and unlock
new capabilities. -->

<!-- ### Key Areas:
- Micro-actuators 
- Miniaturized power system
- Advanced manufacturing techniques
- Integration methodologies

### Active Development:
- MEMS-based actuators
- Smart material applications
- Micro-scale power systems
- Compact sensing solutions -->

</div>

---
<!-- 
*Research collaborations and funding opportunities are welcome. Please contact for more information.* -->