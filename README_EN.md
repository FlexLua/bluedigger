# BlueDigger

[中文](README.md) | [English](README_EN.md)

<p align="center">
  <img src="pic/IMG_2658.webp" alt="BlueDigger" width="480">
</p>

This project uses FlexLua's CPU-302 AI auto-programming control unit, so you can make the 302 do what you want without coding. The 3D printing files are open-source and can be printed with a Bambu Lab 3D printer. Learn more about FlexLua at [flexlua.com](https://flexlua.com).

---

## Project 1: Phone Remote Control

<img src="pic/mobile_control.webp" alt="Phone Remote Control" width="360">

### Project Introduction

This project controls the excavator's actions (forward/backward/left/right movement + bucket flipping) via the "Remote Button Group" widget in a phone Bluetooth App / Mini Program.

**Project video:** https://www.bilibili.com/video/BV1rQbL69Evz/

**The following conditions must be met to run this project:**

1. Have CPU-302 and related accessories ready.
2. In the App, check "Terminal", and add two "Remote Button Group" widgets in the Y0 and Y1 areas of the Terminal page to control the excavator's forward/backward/left/right movement and bucket flipping.

### Pre-description

```
I built an excavator. M1 is connected to the left-wheel motor, M0 to the right-wheel motor. When moving forward, both left and right motors rotate forward; when moving backward, both rotate reverse. When turning left, the right motor rotates forward and the left motor rotates reverse, both at full speed, and so on. P0 is connected to the boom servo, P1 to the arm servo, V0 to the headlights (press once to turn on, press again to turn off). After power-on, both boom and arm servos start at the maximum angle of 180°. During motion, the boom servo angle must never go below 120°.
```

### AI Prompt 1

```
Help me implement phone remote control for the excavator.
```

---

## Project 2: Headlights + Wheels + Forward/Backward Motion Control

<img src="pic/light.webp" alt="Headlight Control" width="360">

### Project Introduction

Three examples demonstrate how to make the excavator automatically flash its headlights, wiggle its wheels left and right, and move forward/backward.

**Project video:** https://www.bilibili.com/video/BV1kQbL69EPT/

**The following conditions must be met to run this project:**

1. Have CPU-302 and related accessories ready.

### Pre-description

```
I built an excavator. M1 is connected to the left-wheel motor, M0 to the right-wheel motor. When moving forward, both left and right motors rotate forward; when moving backward, both rotate reverse. When turning left, the right motor rotates forward and the left motor rotates reverse, both at full speed, and so on. P0 is connected to the boom servo, P1 to the arm servo, V0 to the headlights (press once to turn on, press again to turn off). After power-on, both boom and arm servos start at the maximum angle of 180°. During motion, the boom servo angle must never go below 120°.
```

### AI Prompt 1

```
Flash the headlights 10 times in a row.
```

### AI Prompt 2

```
Wiggle the excavator's wheels left once, then right once, repeat this back-and-forth three times, then stop and stay still.
```

### AI Prompt 3

```
Move the excavator forward for 3 seconds, then backward for 3 seconds, and repeat this cycle twice.
```

---

## Project 3: Excavator Dance

<img src="pic/dance.webp" alt="Excavator Dance" width="360">

### Project Introduction

Have the excavator generate its own code to create a dancing effect.

**Project video:** https://www.bilibili.com/video/BV1kQbL69EA1/

**The following conditions must be met to run this project:**

1. Have CPU-302 and related accessories ready.

### Pre-description

```
I built an excavator. M1 is connected to the left-wheel motor, M0 to the right-wheel motor. When moving forward, both left and right motors rotate forward; when moving backward, both rotate reverse. When turning left, the right motor rotates forward and the left motor rotates reverse, both at full speed, and so on. P0 is connected to the boom servo, P1 to the arm servo, V0 to the headlights (press once to turn on, press again to turn off). After power-on, both boom and arm servos start at the maximum angle of 180°. During motion, the boom servo angle must never go below 120°.
```

### AI Prompt 1

```
Help me write code that makes the excavator start dancing.
```

---

## Technical Exchange

- WeChat: stdlib-h
- Email: shineblink666@gmail.com
