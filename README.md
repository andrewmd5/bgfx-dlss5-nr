# DLSS5-NR for Borderless Gaming

Bring a new look to familiar games. DLSS5 neural rendering, optimized for Borderless Gaming—with adjustable lighting, tone and structure, on more than just the latest NVIDIA GPUs.

The latest release includes **Small and Large models together**. Choose Small for lower GPU cost, or Large for the stronger look of the original model. Both have Standard and Natural presets and include DirectX 12 optimizations for the RTX 3090 and Intel Arc B580.

[Get Borderless Gaming on Steam](https://store.steampowered.com/app/388080/Borderless_Gaming/) · [Download the effect](https://github.com/andrewmd5/bgfx-dlss5-nr/releases/latest)

<table>
  <tr>
    <td width="33%" align="center" valign="bottom">
      <a href="images/niko.png"><img src="images/niko-preview.png" alt="Niko in GTA IV — original left, DLSS5-NR right" width="300" /></a>
    </td>
    <td width="33%" align="center" valign="bottom">
      <a href="images/arthur.png"><img src="images/arthur-preview.png" alt="Arthur in Red Dead Redemption 2 — original left, DLSS5-NR right" width="300" /></a>
    </td>
    <td width="33%" align="center" valign="bottom">
      <a href="images/sora.png"><img src="images/sora.png" alt="Sora — original left, DLSS5-NR right" width="300" /></a>
    </td>
  </tr>
  <tr>
    <td align="center">GTA IV</td>
    <td align="center">RDR2</td>
    <td align="center">Sora</td>
  </tr>
  <tr>
    <td colspan="3" align="center">Original Large model examples · OFF / ON · Strength 1 · Local tone 1.5 · Structure 2 · Natural · Resolution 950</td>
  </tr>
</table>

## Install

Requires **Borderless Gaming 2.0.12 or newer**. If you used an earlier NR package, update the app and reinstall the effect using these steps.

1. Open the effects editor in Borderless Gaming, or the presets screen in Holo.
2. Choose **Install from GitHub** and paste `https://github.com/andrewmd5/bgfx-dlss5-nr`.
3. Select a **DLSS5-NR (Small)** or **DLSS5-NR (Large)** preset and enable effects. On Windows, use **Clone**.

That's it—Borderless Gaming handles the download and setup. No DLLs to copy, no game files to change, and no extra tools to install. Start with the included settings and adjust the look to your taste.

| Preset | Model and appearance |
| --- | --- |
| DLSS5-NR (Small) | Smaller 310.9.16 model, Standard style |
| DLSS5-NR (Small, Natural) | Smaller model, Natural style |
| DLSS5-NR (Large) | Original larger model, Standard style |
| DLSS5-NR (Large, Natural) | Original larger model, Natural style |

Existing NR presets continue to use Small after updating. Both models are installed together; switching presets selects the model. The release also includes separate Small and Large `.bgfxo` files for manual use.

Small includes corrections to intermediate rounding and attention calculations. Large keeps the original model's appearance while benefiting from DirectX 12 optimizations. The models can produce different lighting, tone and detail at the same settings.

Inference size is adjustable from 320 to 1920 and defaults to 960. The shader package uses DirectX 12 or Vulkan, depending on your renderer and GPU capabilities. DirectX requires Shader Model 6.10 and compatible matrix operations; Vulkan requires compatible cooperative-matrix operations. BGFX checks support before enabling the effect.
