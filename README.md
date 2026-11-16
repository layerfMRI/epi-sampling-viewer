<img src="assets/icon.svg" width="64" height="64" alt="">

# EPI k-space sampling viewer

Interactive viewer of which (ky, kz) phase-encode lines are acquired in 3D-EPI with
2D-CAIPIRINHA undersampling and k-space segmentation, given four protocol parameters:
acceleration Ry, acceleration Rz, CAIPI shift Δz and segmentation factor S.
Hover/click a sample to see all lines acquired within the same shot (in echo order);
"Play" animates the acquisition order.

**Live:** https://layerfmri.github.io/epi-sampling-viewer/

## Files

- `epi-sampling-viewer.html` – self-contained snippet (no external libraries). Paste it into a
  WordPress *Custom HTML* block (self-hosted WordPress).
- `index.html` – the same snippet wrapped as a full page, served by GitHub Pages. Embed it with
  `<iframe src="https://layerfmri.github.io/epi-sampling-viewer/" style="width:100%;height:1000px;border:0"></iframe>`.
  After editing the snippet, regenerate `index.html` so both stay in sync.

## Reference

Sampling model and z-blip equations follow Stirnberg R, Stöcker T. *Segmented K-Space
Blipped-Controlled Aliasing in Parallel Imaging (Skipped-CAIPI) for High Spatiotemporal
Resolution Echo Planar Imaging.* Magn Reson Med 2020. doi:10.1002/mrm.28486 —
original notebook: https://github.com/mrphysics-bonn/skipped-caipi
