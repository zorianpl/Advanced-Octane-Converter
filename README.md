The addon attempts to convert all Cycles Materials in the scene to Octane Materials. The Octane shader tree is alongside the Cycles shader, allowing both engines to be used simultaneously.

1. Texture Nodes:
   - Convert texture nodes from Cycles to Octane, alongside Cycles shaders.
   - Convert Gamma Settings based on their names.
   - Invert the glossiness texture to function as Roughness.
   - Evertime when is detects Alpha slot used in Cycles Color Texture it bring Alpha Octane Image 

2. Color Ramp Nodes:
   - Convert Color Ramp to Octane Gradient Node.
   - Transfer colors and positions from the original Color Ramp.

3. Convert Color Mix Texture from Cycles to Octane (currently without Value).

4. Convert Hue Saturation Value to Color Correction nodes with corresponding values.

The script introduces predefined material presets and connects textures to them. Based on the textures, it attempts to apply Transmission/Metal/Glass presets; if this fails, a basic preset is used.


  




Check Releases for the latest version : 

https://github.com/zorianpl/Advanced-Octane-Converter/releases
