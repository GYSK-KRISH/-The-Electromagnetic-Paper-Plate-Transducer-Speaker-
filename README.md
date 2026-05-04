# -The-Electromagnetic-Paper-Plate-Transducer-Speaker-

## 🎞️ Animated Diagram (SVG with Vibration + Current Flow)

```svg id="speaker-animated"
<svg width="520" height="620" viewBox="0 0 520 620" xmlns="http://www.w3.org/2000/svg">

  <style>
    .label { font-size: 12px; font-family: Arial, sans-serif; }
    .title { font-size: 18px; font-weight: bold; }
  </style>

  <!-- Title -->
  <text x="260" y="30" text-anchor="middle" class="title">
    Electromagnetic Paper Plate Speaker (Animated)
  </text>

  <!-- SOUND WAVES (animated opacity) -->
  <path d="M160 80 Q260 30 360 80" stroke="#555" fill="none">
    <animate attributeName="opacity" values="0.2;1;0.2" dur="1s" repeatCount="indefinite"/>
  </path>
  <path d="M170 100 Q260 50 350 100" stroke="#777" fill="none">
    <animate attributeName="opacity" values="1;0.2;1" dur="1s" repeatCount="indefinite"/>
  </path>
  <text x="260" y="70" text-anchor="middle" class="label">Sound Waves</text>

  <!-- GROUP: vibrating system -->
  <g>
    <!-- VIBRATION ANIMATION -->
    <animateTransform attributeName="transform"
      type="translate"
      values="0,-3; 0,3; 0,-3"
      dur="0.15s"
      repeatCount="indefinite"/>

    <!-- Paper Plate -->
    <ellipse cx="260" cy="140" rx="120" ry="30" fill="#e3f2fd" stroke="#000"/>
    <text x="260" y="145" text-anchor="middle" class="label">
      Paper Plate (Diaphragm)
    </text>

    <!-- Voice Coil -->
    <rect x="220" y="170" width="80" height="40" fill="#ffe082" stroke="#000"/>
    <text x="260" y="195" text-anchor="middle" class="label">Voice Coil</text>
  </g>

  <!-- AIR GAP -->
  <line x1="260" y1="210" x2="260" y2="240" stroke="#000" stroke-dasharray="4"/>
  <text x="280" y="230" class="label">Air Gap</text>

  <!-- MAGNET -->
  <rect x="210" y="240" width="100" height="50" fill="#c8e6c9" stroke="#000"/>
  <text x="260" y="270" text-anchor="middle" class="label">
    Neodymium Magnet
  </text>

  <!-- BASE -->
  <rect x="160" y="310" width="200" height="60" fill="#eeeeee" stroke="#000"/>
  <text x="260" y="345" text-anchor="middle" class="label">
    Base Structure
  </text>

  <!-- SUPPORTS -->
  <line x1="140" y1="150" x2="160" y2="310" stroke="#000"/>
  <line x1="380" y1="150" x2="360" y2="310" stroke="#000"/>
  <text x="100" y="240" transform="rotate(-90 100,240)" class="label">
    Flexible Supports
  </text>

  <!-- CURRENT FLOW WIRES -->
  <!-- LEFT WIRE (FORWARD CURRENT - RED) -->
  <line x1="220" y1="190" x2="90" y2="190" stroke="red" stroke-width="2">
    <animate attributeName="stroke-dasharray" values="0,10;10,0" dur="0.5s" repeatCount="indefinite"/>
  </line>
  <polygon points="90,190 100,185 100,195" fill="red"/>
  <text x="40" y="185" class="label" fill="red">Forward Current (L/R)</text>

  <!-- RIGHT WIRE (REVERSE CURRENT - BLUE) -->
  <line x1="300" y1="190" x2="430" y2="190" stroke="blue" stroke-width="2">
    <animate attributeName="stroke-dasharray" values="10,0;0,10" dur="0.5s" repeatCount="indefinite"/>
  </line>
  <polygon points="430,190 420,185 420,195" fill="blue"/>
  <text x="360" y="185" class="label" fill="blue">Reverse Current (GND)</text>

</svg>
```

---
