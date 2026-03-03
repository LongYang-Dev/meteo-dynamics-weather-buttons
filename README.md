# ⚡ Meteo-Dynamics — Weather Button Kit

> **11 physics-based animated weather buttons for Android Jetpack Compose.**  
> Drop-in components. Zero dependencies. 60 FPS.

&nbsp;

![Storm Button Demo](assets/storm_button.gif)

&nbsp;

---

## 🌦 What's Inside

11 fully animated, physics-simulated UI buttons — each one a living weather phenomenon:

| # | Button | Effect |
|---|--------|--------|
| 1 | **StormButton** | Violet lightning arcs + electric border |
| 2 | **RainButton** | Physics raindrops + surface ripples |
| 3 | **SnowButton** | Wobbling snowflakes + accumulation layer |
| 4 | **FireButton** | Additive-blend flame particles |
| 5 | **FogButton** | Layered mist with depth parallax |
| 6 | **WindButton** | Curved wind streaks + turbulence |
| 7 | **NightButton** | Moon texture + 180 twinkling stars |
| 8 | **ClearDayButton** | GPU-cached sun rays + lens flare |
| 9 | **OvercastButton** | Pre-baked cloud layers |
| 10 | **HurricaneButton** | Spiral particle vortex |
| 11 | **NeonLightningButton** | Gradient border + cyan lightning path |

---

## 🔌 API at a Glance

Every button shares the same minimal interface:

```kotlin
StormButton(
    text = "GET STARTED",   // customizable label
    onClick = { /* ... */ }
)
```

Plug directly into any Jetpack Compose layout. No setup, no theme changes required.

---

## 📦 Live Weather Integration (Optional)

```kotlin
// OpenWeatherMap example
val weatherCode = response.weather[0].id
val button = when (weatherCode) {
    in 200..232 -> { StormButton(onClick = action) }
    in 300..531 -> { RainButton(onClick = action) }
    in 600..622 -> { SnowButton(onClick = action) }
    800        -> { ClearDayButton(onClick = action) }
    else       -> { OvercastButton(onClick = action) }
}
```

---

## 💳 Purchase & Download

**The full source code (all 11 `.kt` files + assets + README) is available here:**

<a href="https://yanglong.gumroad.com/l/hxjcx">
  <img src="https://img.shields.io/badge/Buy%20on%20Gumroad-%24%2029-FF90E8?style=for-the-badge&logo=gumroad&logoColor=white" alt="Buy on Gumroad" />
</a>

---

## ⚙️ Requirements

- Android API 26+
- Jetpack Compose 1.5+
- Kotlin 1.9+

---

## 📄 License

Commercial license included with purchase. See `LICENSE.txt` in the package.  
© 2026 Meteo Dynamics. All rights reserved.
