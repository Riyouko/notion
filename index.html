<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Leaf Button</title>
<style>
  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: #0d0d12;
    font-family: 'Georgia', serif;
    overflow: hidden;
  }

  /* ── Button wrapper ── */
  .btn-wrap {
    position: relative;
    display: inline-block;
    cursor: pointer;
    user-select: none;
  }

  .btn-wrap img {
    display: block;
    width: 220px;
    height: auto;
    border-radius: 18px;
    transition: transform 0.12s cubic-bezier(.4,2,.6,1), filter 0.15s;
    filter: drop-shadow(0 0 18px rgba(160,80,255,0.35));
  }

  /* Click press-down */
  .btn-wrap:active img,
  .btn-wrap.pressed img {
    transform: scale(0.91);
    filter: drop-shadow(0 0 32px rgba(180,80,255,0.85)) brightness(1.15);
  }

  /* ── Leaf particle ── */
  .leaf {
    position: fixed;
    pointer-events: none;
    width: 18px;
    height: 22px;
    border-radius: 60% 10% 60% 10%;
    background: linear-gradient(135deg, #c060ff, #7b2fff);
    opacity: 0;
    transform-origin: center bottom;
    animation: leafFly 1.1s ease-out forwards;
    z-index: 9999;
  }

  /* Vein line inside leaf */
  .leaf::after {
    content: '';
    position: absolute;
    top: 50%; left: 50%;
    width: 1px; height: 60%;
    background: rgba(255,255,255,0.35);
    transform: translate(-50%, -50%) rotate(15deg);
    border-radius: 2px;
  }

  @keyframes leafFly {
    0%   { opacity: 1; transform: translate(0, 0) rotate(0deg) scale(1); }
    40%  { opacity: 0.9; }
    100% { opacity: 0; transform: translate(var(--tx), var(--ty)) rotate(var(--rot)) scale(0.4); }
  }

  /* ── Ripple ring ── */
  .ripple {
    position: fixed;
    pointer-events: none;
    border-radius: 50%;
    border: 2px solid rgba(160, 60, 255, 0.7);
    transform: translate(-50%, -50%) scale(0);
    animation: rippleOut 0.7s ease-out forwards;
    z-index: 9998;
  }

  @keyframes rippleOut {
    to { transform: translate(-50%, -50%) scale(4); opacity: 0; }
  }
</style>
</head>
<body>

<div class="btn-wrap" id="btn">
  <img src="https://cdn.phototourl.com/free/2026-06-07-1357f2f0-09d7-4c5a-89c3-5948ff27eda1.webp" alt="button">
</div>

<script>
  const btn = document.getElementById('btn');

  btn.addEventListener('click', (e) => {
    const rect = btn.getBoundingClientRect();
    const cx = rect.left + rect.width / 2;
    const cy = rect.top + rect.height / 2;

    // Press animation
    btn.classList.add('pressed');
    setTimeout(() => btn.classList.remove('pressed'), 180);

    // Ripple
    const rip = document.createElement('div');
    rip.className = 'ripple';
    rip.style.cssText = `left:${cx}px;top:${cy}px;width:${rect.width}px;height:${rect.width}px`;
    document.body.appendChild(rip);
    rip.addEventListener('animationend', () => rip.remove());

    // Leaves — burst in all directions
    const count = 14;
    for (let i = 0; i < count; i++) {
      const leaf = document.createElement('div');
      leaf.className = 'leaf';

      // Random spread angle (mostly upward: -150° to -30°)
      const angle = (Math.random() * 300 - 240) * (Math.PI / 180);
      const dist  = 80 + Math.random() * 130;
      const tx = Math.cos(angle) * dist;
      const ty = Math.sin(angle) * dist;
      const rot = (Math.random() - 0.5) * 540;
      const size = 12 + Math.random() * 14;

      // Slight color variation
      const hue = 270 + (Math.random() - 0.5) * 40;
      leaf.style.cssText = `
        left: ${cx}px;
        top: ${cy}px;
        width: ${size}px;
        height: ${size * 1.25}px;
        --tx: ${tx}px;
        --ty: ${ty}px;
        --rot: ${rot}deg;
        animation-delay: ${Math.random() * 0.08}s;
        animation-duration: ${0.9 + Math.random() * 0.5}s;
        background: linear-gradient(135deg, hsl(${hue},90%,70%), hsl(${hue + 20},80%,45%));
        transform: translate(-50%, -50%);
      `;
      document.body.appendChild(leaf);
      leaf.addEventListener('animationend', () => leaf.remove());
    }

    // Navigate after animation
    setTimeout(() => {
      window.location.href = 'page2.html'; // ← change this to your target URL
    }, 500);
  });
</script>
</body>
</html>