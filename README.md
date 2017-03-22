### WebGL Memory Stress Test

Create WebGL textures until running out of memory.

IE, Edge and FireFox return the correct error (gl.OUT_OF_MEMORY), and allow for recovery.

Chrome returns gl.CONTEXT_LOST_WEBGL and does not allow recovery. 

Any further WebGL call will prompt "Rats! WebGL hit a snag", and the user must reload the page.

documented with chromium with issue <a href="https://bugs.chromium.org/p/chromium/issues/detail?id=93857">93857</a>
