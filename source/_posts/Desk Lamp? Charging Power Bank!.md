---
abbrlink: Desk Lamp? Charging Power Bank!
categories:
- - This Blog
- - Meaningless Works
date: '2024-10-24T22:04:40.112121+08:00'
tags:
- Develop
title: Charging Power Banks That Don't Want to Shine Aren't Good Desk Lamps
updated: '2024-10-24T22:06:46.679+08:00'
---
# Charging Power Banks That Don't Want to Shine Aren't Good Desk Lamps

## Why Did This Idea Come About?

When I was young, I once traveled to Xishuangbanna, China. At that time, while packing, there was a rule from the Civil Aviation Administration of China that the total capacity of power banks carried on board couldn't exceed 20,000mAh. I wanted to bring both a 20,000mAh power bank and a 20,000mAh desk lamp. However, according to the rules, I couldn't bring both, so I was forced to make a decision: I chose the power bank.

This resulted in a situation where, during my time in Xishuangbanna, I was working on my computer organizing the photos I took during the day, but my mother preferred to sleep early. If I had brought the desk lamp, I could have sorted the photos at night without disturbing her. However, if I had brought the lamp, my camera would have run out of battery on the way. So, I had this idea: **add charging functionality to the desk lamp**.

## My Preparations + Initial Idea

Initially, I thought of adding an outward charging port to the desk lamp with a large built-in capacity, so I planned to purchase a charging board for external output. The schematic was as follows:

- When the battery serves as the power source output, it simultaneously supplies power to the parallel output control board and the lamp control board at 3.7V, allowing both to work without interference.
- When charging, the battery accumulates energy as an electric appliance. The overall concept looked like this:

![Schematic Diagram](https://img.picui.cn/free/2024/10/24/671a4faef3d9f.png)

Electricity enters through the newly added charging control board, providing power to both the battery and the desk lamp control board. Quite ingenious!

Being a keen enthusiast, I enjoy pushing limits in everything I do. So, this time I decided to upgrade the added charging board to a **60W power output**, giving the lamp the capability to emergency charge my MacBook Air.

Although this might sound outrageous, I decided to give it a try. First, I disassembled my desk lamp. The interior looked like this:

![Desk Lamp Interior](https://img.picui.cn/free/2024/10/24/671a4fb21697a.png)

The green circuit board represents the lamp's control circuit, the silver part is the battery, and yellow adhesive tape is wound around the sides.

I found a charging board on the internet that could handle both 60W charging and discharging, and it was tiny. A friend who had used this charging board to modify his charger told me it was very efficient. So, I invested heavily and acquired one. It looked very compact and had excellent circuit protection – almost tailor-made for this project. It looked like this:

![Charging Board](https://img.picui.cn/free/2024/10/24/671a4fe1d24c8.png)

After some calculations, I realized this component was taller than what my desk lamp could accommodate. So, now I had two options:

1. Cut down the existing backplate to fit this 'massive' charging control board, or
2. 3D print a new one.

I found the cutting option to be visually unappealing, as I'm not a fan of such makeshift solutions. Therefore, I chose the latter. Additionally, I noticed that when using the new charging board for charging, the total circuit voltage would rise to 4.2V. The original relationship between the desk lamp's battery and the charging board was as follows: the protection board was integrated onto the lamp's control board. The battery's maximum output voltage was 3.7V, so the manufacturer set the input voltage limit to 3.7V. Any voltage exceeding this would pose a danger.

So, I made a clever move: I connected a voltage converter. However, I couldn't find a high-power 4.2V to 3.7V converter on the market, and personal customization was unfeasible. Hence, I came up with a truly ingenious idea: **step up the voltage first, then step it down**. The voltage transformation looked like this: 4.2V transformed to 15V, then to 3.3V. It looked like this:

![Voltage Transformation](https://img.picui.cn/free/2024/10/24/671a4fe1aece3.png)

Though it might seem a bit outlandish, the actual experience was quite positive. The two-layer nesting for high power was implemented to prevent sudden high voltage from damaging the transformer, and the efficiency was around **85%**, which is pretty good.

I used software called **'3D One'** for modeling, and for the first time, I completed the entire process in this project. Throughout the process, there were a total of four versions of the casing. Apart from the first version, which took five days of tinkering with a friend's help to print, the other three versions were all printed by platform services, yielding results much better than what my friend achieved.

The final result looked like this: **perfect**. No overheating, and all of the desk lamp's functions remained intact. This, my friends, is the true desk lamp!
