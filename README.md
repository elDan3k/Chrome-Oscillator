# Chrome-Oscillator

Epic chrome built-in oscillator effect in few simple steps. Open new chrome tab an type in console:
```
  let ctx = new AudioContext()
  let osc = ctx.createOscillator()
  osc.connect(ctx.destination)
  window.onmousemove = event => {osc.detune.value = event.clientY; osc.frequency.value = event.clientX}
  
  osc.start()
  osc.stop()
```
