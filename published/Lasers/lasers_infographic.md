# How a Laser Works, From A to Z

So I wanted to learn how a laser actually works, from the basic level all the way down to the fundamental level. I researched it and explained it in my own words. If you came here from my LinkedIn post, this is the in-depth version with all the small details and nudges that I didn't mention there.

![Inside a laser: two mirrors, the gain medium, the pump, and the beam leaking out of the 95% mirror](Lasers/laser-diagram.png)

---

## The Short Version

When you click the power on button on a laser, what happens inside is that the electricity from the battery excites the electrons of a specific material up to a specific level. Once they're at the right level, one of the electrons drops down, and the moment it does, it produces a photon. That photon hits one of the mirrors inside the laser, reflects back into the middle, which is where the excited electrons are, and gets doubled. And it just keeps bouncing back and forth between these two mirrors.

The reason I say two mirrors is because in a laser, there are two mirrors on two ends. One is 100% reflective and one is 95% reflective. The reason one of them is 95% reflective is because some of the light needs to escape to show up as a beam, and that beam is what you see as the laser.

The reason that light is coherent is, think of it like an army. When you see soldiers in the army, they're all walking in step, at the same time, at the same speed, right? That's what the photons in a laser do. It takes that one photon that came out of the electron and turns it into many copies, all doing everything in step.

All of this happens in a billionth of a second. That's why when you click it, you see the beam immediately. And the reason it doesn't get any brighter is because the excited electrons get refilled by the electricity as fast as the photons use them up. That's why you see the same brightness level the moment you click the power on button.

---

## Contents

1. [Energy Levels](#1-energy-levels)
2. [The Three Ways Light and Atoms Interact](#2-the-three-ways-light-and-atoms-interact)
3. [Population Inversion](#3-population-inversion)
4. [The Four Levels](#4-the-four-levels)
5. [The Mirrors (Optical Cavity)](#5-the-mirrors-optical-cavity)
6. [Threshold](#6-threshold)
7. [What Makes Laser Light Special](#7-what-makes-laser-light-special)
8. [What's the Material in the Middle?](#8-whats-the-material-in-the-middle)
9. [Where the Heat Comes From](#9-where-the-heat-comes-from)
10. [Quick Notes](#10-quick-notes)
11. [Quick Glossary](#11-quick-glossary)

---

## 1. Energy Levels

So basically, in an atom, there is a nucleus in the middle, and around the nucleus there are electrons. Each electron has its own specific level. It's not shells really, it's different energy levels, kind of like rungs on a ladder. The key thing is that electrons can only have a certain specific amount of energy, never anything in between. So for an electron to jump between levels, it needs a specific amount of energy put into it.

When an electron gets excited, it jumps up between levels, and there are different gaps when it jumps. When it falls back down, the energy has to go somewhere. And since a photon is a packet of energy, it comes out as light.

That gap determines how much energy comes out, and that energy determines the wavelength. A big gap means high energy, and high energy means a short wavelength. That short wavelength is on the blue side. When the gap is smaller, there's less energy, which means a longer wavelength, and that's closer to red. That's how you determine the color of a laser, or of anything really, because the energy comes from the gap between the energy levels.

| Gap | Energy | Wavelength | Color |
|---|---|---|---|
| Big | High | Short | Blue / violet |
| Medium | Medium | Medium | Green / yellow |
| Small | Low | Long | Red |
| Even smaller | Lower | Longer | Infrared (can't see it) |

The easy way I remember it: high energy light is excited, so it wiggles fast with short, choppy waves. That's blue. Low energy light is lazy, with long, slow waves. That's red.

And outside of what we can see, on the low end it's radio, then infrared, which is your TV remote for instance. Then it's the visible colors from red to violet, then UV, then X-rays on the high end.

```
 LOW ENERGY                                                   HIGH ENERGY
 long waves                                                   short waves

 Radio ─── Infrared ─── [ Red  Orange  Yellow  Green  Blue  Violet ] ─── UV ─── X-rays
           (TV remote)          visible light (what we can see)
```

---

## 2. The Three Ways Light and Atoms Interact

There are three different ways light and atoms interact: absorption, spontaneous emission, and stimulated emission.

**Absorption** is when the photon is getting eaten by an electron. But it can't just be eaten, right? It has to match the same size as the gap to get the electron excited.

**Spontaneous emission** is when an excited electron randomly drops down to a lower level on its own, and the photon goes in a random direction. It's a completely new photon, but it goes in a random direction. This is where the very first photon in a laser comes from.

**Stimulated emission** is the idea behind what Albert Einstein came up with back in 1917. A photon hits an already excited electron, and that just nudges it to drop down. And it comes out as a perfect clone, at the same energy level and the same direction, in phase. So that dropped photon doubles it, at the same level, the same speed, the same direction, in step with the photon that just passed by it. It's basically one coming in and two coming out.

And that's where the SE in laser comes from: **L**ight **A**mplification by **S**timulated **E**mission of **R**adiation.

| Type | What happens | Which direction the photon goes |
|---|---|---|
| Absorption | The photon gets eaten and the electron jumps up | No photon comes out |
| Spontaneous emission | The electron randomly drops on its own | Random |
| Stimulated emission | A photon nudges an already excited electron to drop | Same exact direction as the photon that nudged it |

Easy way to remember it: spontaneous means it happens on its own, stimulated means something nudges it.

---

## 3. Population Inversion

Population inversion is when there are more excited electrons than calm electrons. The reason we need that is because we need stimulated emission for the laser to work properly. If most of the electrons are calm, the photons just get eaten instead of cloned.

So why can't you just use two levels? With two levels, it's basically 50-50 of the excited electrons and the calm electrons, and the eating and the cloning cancel each other out. You never get more excited than calm. That's why lasers use three or four levels instead.

---

## 4. The Four Levels

The first step is the electricity jumps the electron up to level four. Then from four to three, it releases energy, and that energy comes out as heat, not a photon, because there's not enough energy in that gap. It just comes out as heat.

Then from three to two is when the actual photon happens. A passing photon stimulates this drop, and this is the only gap that makes laser photons. So that's what sets the laser's color.

And then there's the fast drop from two to one. That's another heat sink, which doesn't produce any photon. The gap isn't big enough, so it just produces some low level energy that turns into heat, which goes into the material. That's why you feel the heat on the laser when it's on.

```
  Level 4   ━━━━━━━━━━━━━━━━━━━━━   ← electricity jumps it up here
                    │
                    │  drop → heat, not a photon
                    ▼
  Level 3   ━━━━●━●━●━●━●━●━●━━━━   ← sticky: the electrons pile up here
                    │
                    │  THE LASER DROP → photon (this gap sets the color)
                    ▼
  Level 2   ━━━━━━━━━━━━━━━━━━━━━   ← empties out fast
                    │
                    │  drop → heat, not a photon
                    ▼
  Level 1   ━━━━━━━━━━━━━━━━━━━━━   ← calm (ground state)

      ▲
      └── then the electricity jumps it back up to level 4 and it goes again
```

| Step | From → To | What comes out |
|---|---|---|
| 1 | Level 1 → Level 4 (up) | Nothing, the electricity puts energy in |
| 2 | Level 4 → Level 3 | Heat |
| 3 | Level 3 → Level 2 | **The laser photon** |
| 4 | Level 2 → Level 1 | Heat |

So each electron gives one laser photon per trip, then it gets jumped back up and goes again.

### Why level three is "sticky"

Level three is sticky, meaning the electrons hang around there way longer before they drop, so they pile up. That's called **metastable**. On a normal level, an electron drops in a few billionths of a second. On level three, it waits thousands to millions of times longer.

So why does the drop even happen eventually? It's basically luck. The electron doesn't have a timer, it just has a chance of dropping every moment, like rolling dice over and over. On level three, the odds are just way worse, so it waits longer.

And that's actually why the pile up matters. Electrons pour in fast from level four and drain out slow from level three, kind of like a bathtub, so they pile up. That pile is the population inversion. Then a passing photon comes in and makes them drop on demand instead of waiting for luck.

---

## 5. The Mirrors (Optical Cavity)

The two mirrors together, plus the area between them, are called the **optical cavity**, or the **resonator**.

The light needs to bounce around something, because if it just travels one way, it won't be much of a beam. Its losses would be much higher than its gains. So the mirrors keep reflecting the photons back and forth, and every time they pass through the material in the middle, they get cloned. The mirrors don't do the cloning, the material does. The mirrors just keep sending the light back through it.

Some photons go in random directions. That's why you lose the photons that are going at an angle. They get absorbed by the material on the sides of the laser, which also turns into heat.

That's why when the first photon comes out, it's gotta be lucky. It either goes straight at the mirror or it doesn't. And if it doesn't, there's millions of other electrons that are about to drop, and one of them eventually will. And since all of this happens in billionths of a second, one of the photons is going to hit the mirror straight. Once it does, it starts bouncing back and forth, which is why you get one straight line, the same color, the same damn beam.

And the reason one mirror is 95% reflective is because some of the light needs to escape to show up as the beam.

---

## 6. Threshold

Think of it like filling a bucket with a hole in it. If you're filling the bucket with water at a slower rate than it's leaking, then you won't get a full flow of water from the hole. In this case, that means you won't get a coherent beam, just a weak random glow.

But if you start pouring at a faster rate, the bucket starts to actually fill up. It's still losing water, but it fills up to a certain point, and then it keeps releasing the same level of water flow. In our case, that's a laser, which keeps the same level of beam.

The **threshold** is that exact point where the pouring starts to beat the leaking.

That's why when the battery of a laser dies out, when you're literally trying to point it, it doesn't fade out. It just shuts off. If at any point the losses beat the gains, the laser just stops working, because there's not enough stimulated emission to keep the beam going.

### Why it doesn't get brighter forever

The photons don't keep doubling forever. They multiply up to a certain point, and then it stays the same brightness. That's because the excited electrons get refilled as fast as they're used up. Every clone uses up one excited electron, so once the light is using them up exactly as fast as the electricity refills them, the gains equal the losses, and the brightness stays the same. That's called **gain saturation**.

---

## 7. What Makes Laser Light Special

**One color** is basically the gap level. The gap between the two levels is what determines the color, and since every photon comes from the same gap and every clone copies it, they're all the same color.

**The tight beam** is because it's bouncing between the two mirrors in a straight line, and only the straight ones survive. So it comes out of that 95% mirror as a straight line.

**Coherent** is basically when everything moves in one flow, together, in step. When everything is perfectly aligned. It's like the army example. They're not just the same people doing the same thing, they're following the same rhythm, the same step, at the same time.

| What it is | Fancy name | Why it happens |
|---|---|---|
| One color | Monochromatic | Every photon comes from the same gap |
| Tight beam | Directional | Only the straight photons keep bouncing between the mirrors |
| In step | Coherent | Every clone copies the photon that made it |

And when you hold a laser against a wall, you'll see some grainy, sparkly bits around the dot, but it's still mostly one tight dot. Those sparkly bits are called **speckle**, and it actually happens because the light is so coherent. The rough wall makes the in-step waves bump into each other.

---

## 8. What's the Material in the Middle?

The material in the middle that's getting excited is called the **gain medium**. It depends on the laser:

| Laser | The material in the middle | What excites it |
|---|---|---|
| Red laser pointer | A tiny semiconductor chip, basically a special LED. The chip's ends act as the mirrors. | Electricity |
| Helium-neon (the classic lab laser) | Helium and neon gas in a tube | Electricity |
| Ruby (the very first laser, 1960) | A ruby crystal | A bright flash lamp |

---

## 9. Where the Heat Comes From

At first I thought that if you hold the laser on for a long time, the heat was from the light building up and multiplying inside forever. That's not it. The light levels off almost instantly.

The heat comes from the drops from four to three and from two to one, which come out as heat instead of photons. And it also comes from the photons going at an angle that get absorbed by the sides of the laser.

---

## 10. Quick Notes

- The ends of the laser are **mirrors**, not lenses.
- A photon is a **packet of light energy**, not matter.
- **Photons** are the ones bouncing between the mirrors, not electrons. The electrons never leave the material.
- Coherent means the photons are **in step**. The straight line is a result of that.
- The light doesn't keep doubling forever. It levels off once the excited electrons get refilled as fast as they're used up.
- A laser turns on in **billionths of a second**.
- The speed of light is about **300 million meters per second** (299,792,458 m/s to be exact).

---

## 11. Quick Glossary

| Word | What it means |
|---|---|
| Photon | A packet of light energy |
| Energy level | A specific rung an electron can sit on |
| Ground state | The lowest level, where the electron is calm |
| Excited state | Any level above the calm one |
| Absorption | The photon gets eaten and the electron jumps up |
| Spontaneous emission | The electron drops on its own, photon goes in a random direction |
| Stimulated emission | A photon nudges an excited electron down, and a perfect clone comes out |
| Population inversion | More excited electrons than calm ones |
| Metastable | A sticky level where electrons pile up |
| Pump | Whatever excites the electrons, like electricity |
| Gain medium | The material in the middle that gets excited |
| Optical cavity | The two mirrors and the space between them |
| Threshold | The point where the gains start to beat the losses |
| Gain saturation | When the brightness stops growing and stays the same |
| Coherent | The photons are in step with each other |

---

*If you see something I got wrong, leave a comment or open an issue. If I don't have the answer, I'll research more into it and come back.*