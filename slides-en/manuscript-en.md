# Secrets of Rhythm Unveiled by the Kuramoto Model: Why Does Applause Synchronize?

## 01-Title Slide

Today I'll be talking about "Secrets of Rhythm Unveiled by the Kuramoto Model. We'll explore the phenomenon of "Why Does Applause Synchronize?" from a mathematical modeling perspective.

## 02-About Me

Let me briefly introduce myself. I'm Same, also known as мег-сск, and I work as a freelance software engineer. I'm currently also studying at an online university as a working professional.

My areas of expertise are mainly three: Computer Vision, where I work with image recognition and point cloud processing; Spatial Information Processing, including GIS and remote sensing; and Cloud Infrastructure Design using AWS and GCP with Infrastructure as Code practices.

I also share information on GitHub, YouTube, and Speaker Deck, so please check those out if you're interested.

## 03-Today's Topics

Today, I'll be covering the following topics:

First, I'll introduce the Kuramoto model, which can model synchronization phenomena - when random rhythms align with each other.

Next, I'll break down the meaning of the Kuramoto model's equation. The equation might look complex at first glance, but it's actually quite intuitive, so don't worry.

Then, we'll observe a simulation of the Kuramoto model recreating "firefly flashing" patterns.

Finally, I'll discuss the Kuramoto conjecture and the critical coupling constant, along with introducing representative examples of "phase transitions."

## 04-Overview of the Kuramoto Model

Now, let's delve into what the Kuramoto model is all about.

## 05-What is the Kuramoto Model?

The Kuramoto model is a mathematical model designed to describe phenomena where rhythms synchronize. It was proposed by Dr. Yoshiki Kuramoto in 1975.

There's an interesting video I'd like to show you where multiple metronomes placed on the same platform gradually synchronize their rhythms, even though they start off completely out of sync. This is a classic example of synchronization.

## 06-Applications of the Kuramoto Model

The Kuramoto model can model various rhythm synchronization phenomena.

For example, it can model how applause rhythms naturally align during concerts, or how fireflies in a group flash in unison.

Another important application is in power grids, where generator frequencies must remain synchronized. If they fall out of sync, it can lead to major blackouts!

In medicine, the model can also represent heart rhythm patterns, and disruptions in these patterns are related to conditions like atrial fibrillation.

## 07-The Kuramoto Model Equation

Let's look at the Kuramoto model equation.

In this equation, θ_i represents the phase of oscillator i, ω_i is its angular velocity, K is the coupling constant representing interaction strength, and N is the total number of oscillators.

While it might look complex at first, the meaning of this equation is actually quite straightforward.

## 08-Meaning of the Second Term on the Right

The second term on the right is particularly important.

To understand this, think of θ_i as your applause rhythm and θ_j as other people's applause rhythms.

This term represents the average deviation between your rhythm and everyone else's. The larger the coupling constant K, the stronger the correction force for this deviation becomes, making rhythms more likely to synchronize.

## 09-Meaning of the Coupling Constant K

Let me explain more about the coupling constant K.

The larger K is, the more easily rhythms synchronize. Conversely, when K is small, each oscillator tends to maintain its own rhythm, making synchronization difficult.

In the applause example, K can be thought of as quantifying how much you're consciously trying to match your applause to others. When K=0, you're not paying any attention to others' applause and just maintaining your own rhythm.

Later on, we'll see in simulations how behavior changes with different values of K.

## 10-Revisiting the Kuramoto Model Equation

Let's look at the Kuramoto model equation once more.

This equation shows that the rate of change of your rhythm is determined by your natural rhythm and the average deviation from others' rhythms.

When the coupling constant K=0, the second term disappears, and you continue moving at your natural rhythm speed ω_i indefinitely.

As K increases, the deviation from others' rhythms has a greater influence on your rhythm's rate of change.

## 11-Simulation of the Kuramoto Model

Now, let's look at simulations of the Kuramoto model.

## 12-Simulating the Kuramoto Model

Kuramoto model simulation code is shared on GitHub, so I modified their code to experiment with it. If you're interested, you can access it via the URL shown on the slide.

Using this code, I simulated how firefly flashing rhythms synchronize. Let's observe how behavior changes with different values of the coupling constant K.

## 13-Firefly Flashing: K=2

First, let's look at the case where K=2.

As you can see, rhythms gradually synchronize over time. The initially random flashing patterns slowly align until they're almost perfectly synchronized.

## 14-Firefly Flashing: K=5

Next, the case where K=5.

With a larger coupling constant, you can see that rhythms synchronize much more quickly. Synchronization occurs much faster than with K=2. This is because the force trying to match others' rhythms is stronger.

## 15-Firefly Flashing: K=0

In contrast, what happens when K=0?

When the coupling constant is 0, meaning fireflies don't respond to others' flashing at all, rhythms never synchronize. Each firefly maintains its own inherent rhythm indefinitely, resulting in a permanently random pattern.

## 16-The Mysterious Behavior of the Coupling Constant

Here's an interesting phenomenon. The system's behavior changes dramatically between K=1.59 and K=1.6.

On the left with K=1.59, no matter how much time passes, the rhythms don't synchronize.

On the right with K=1.6, although it takes time, the rhythms eventually synchronize.

With just a 0.01 difference, the system's behavior changes qualitatively. What does this mean?

## 17-The Kuramoto Conjecture and Phase Transitions

Now let's discuss the Kuramoto conjecture and phase transitions.

## 18-The Kuramoto Conjecture

The Kuramoto conjecture states that when the coupling constant exceeds a critical point K_c, rhythms suddenly begin to synchronize.

It's like water suddenly turning to ice at 0°C. The system's properties change qualitatively at the critical point.

The critical point K_c is expressed by the equation shown on the slide.

Where g(ω) is the distribution function of angular velocities, and g(0) is the value of this function when ω=0.

## 19-Calculating the Critical Point

In our simulation, we used a standard normal distribution with the average at 0 and the standard deviation at 1, as the angular velocity distribution function.

We'll use this distribution's equation to calculate the critical point.

## 20-Mean Field Frequency

The average angular velocity of all oscillators becomes 0. This average angular velocity is called the mean field frequency.

This means the entire system's distribution can be represented by g(0). For a standard normal distribution, g(0) equals 1/√(2π).

## 21-Calculating the Critical Point

Substituting values into our earlier equation, we can get

K_c ≃ 1.596

This explains why rhythms synchronize with K=1.6 but not with K=1.59. K=1.6 just barely exceeds the critical point, enabling synchronization. Meanwhile, K=1.59 falls below the critical point, so synchronization doesn't occur.

This phenomenon, where properties change dramatically beyond a critical point, is called a "phase transition."

## 22-Examples of Phase Transitions

Phase transitions appear in various physical phenomena.

For example, water turning to ice at 0°C or water evaporating at 100°C are classic examples of phase transitions. Another example is magnets losing their magnetism at high temperatures.

On an even grander scale, the beginning of the universe is sometimes explained as a vacuum phase transition.

## 23-Proof of the Kuramoto Conjecture

Finally, let me touch on the history of the Kuramoto model and conjecture.

The Kuramoto model was proposed in 1975, and the Kuramoto conjecture was formulated in 1984.

This conjecture was proven in 2012 by Dr. Hayato Chiba, who was at Kyushu University at the time. A link to the paper is included in the slide for those interested.

Given that it's now mathematically proven, I believe it should be referred to as the "Kuramoto-Chiba Theorem" going forward.

## 24-Summary

To summarize today's talk:

We've seen how the Kuramoto model can explain phenomena where "rhythms synchronize."

The coupling constant represents the tendency to adjust to deviations from surrounding rhythms.

When the coupling constant exceeds the critical point, rhythms suddenly synchronize - this is the Kuramoto conjecture, which was proven in 2012.

The Kuramoto model is a representative model of phase transition phenomena and is applied in various fields.

## 25-Call for Lightning Talk Presenters

The Physics Study Group is looking for lightning talk presenters! Any genre is welcome, so if you're interested, please join the Physics Study Group Discord server.

I've heard that if no one volunteers, the organizer will have to do another "lightning talk" that's actually more like a giant recital... so please consider participating!

## Announcements

Finally, I'd like to announce that the next meeting is scheduled for June 28th.

In addition to lightning talks, we also welcome suggestions for physics YouTube videos that you'd like to watch together with everyone.

That concludes my presentation. Thank you for your attention.
