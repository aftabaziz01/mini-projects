# 🔥 Flame Animation (HTML & CSS)

This project is a pure **HTML and CSS flame animation** that simulates a flickering fire effect using layered div elements, CSS transforms, and keyframe animations.

## 🚀 Project Overview

The flame is built by stacking multiple colored elements:

- 🔴 Red – Outer flame
- 🟠 Orange – Mid layer
- 🟡 Yellow – Inner glow
- ⚪ White – Bright flame core
- 🔵 Blue circle – Flame base glow
- ⚫ Black circle – Shadow/base effect

The flickering effect is created using CSS `@keyframes` animation with slight rotations and scaling to simulate natural fire movement.

## 🛠️ Technologies Used

- HTML5
- CSS3
  - CSS Grid
  - CSS Animations (`@keyframes`)
  - Transforms (`rotate`, `scale`)
  - Box-shadow effects
  - Positioning

## 🎨 How It Works

- The flame layers are absolutely positioned inside a container.
- Each layer uses:
  - `border-radius` for curved shapes
  - `transform: rotate(-45deg)` for flame shaping
  - `box-shadow` for glow effects
- The flicker effect is achieved using:

```css
@keyframes flicker {
  0% { transform: rotate(-1deg); }
  20% { transform: rotate(1deg); }
  40% { transform: rotate(-1deg); }
  60% { transform: rotate(1deg) scaleY(1.04); }
  80% { transform: rotate(-2deg) scaleY(0.92); }
  100% { transform: rotate(1deg); }
}
