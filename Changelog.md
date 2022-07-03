DD54-WithWrap

Created using Colaboratory

#@title <- View Changelog skip_for_run_all = True #@param {type: 'boolean'}

if skip_for_run_all == False: print( ''' v1 Update: Oct 29th 2021 - Somnai

  QoL improvements added by Somnai (@somnai_dreams), including user friendly UI, settings+prompt saving and improved google drive folder organization.
v1.1 Update: Nov 13th 2021 - Somnai

  Now includes sizing options, intermediate saves and fixed image prompts and perlin inits. unexposed batch option since it doesn't work
v2 Update: Nov 22nd 2021 - Somnai

  Initial addition of Katherine Crowson's Secondary Model Method (https://colab.research.google.com/drive/1mpkrhOjoyzPeSWy2r7T8EYRaU7amYOOi#scrollTo=X5gODNAMEUCR)

  Noticed settings were saving with the wrong name so corrected it. Let me know if you preferred the old scheme.
v3 Update: Dec 24th 2021 - Somnai

  Implemented Dango's advanced cutout method

  Added SLIP models, thanks to NeuralDivergent

  Fixed issue with NaNs resulting in black images, with massive help and testing from @Softology

  Perlin now changes properly within batches (not sure where this perlin_regen code came from originally, but thank you)
v4 Update: Jan 2022 - Somnai

  Implemented Diffusion Zooming

  Added Chigozie keyframing

  Made a bunch of edits to processes
v4.1 Update: Jan 14th 2022 - Somnai

  Added video input mode

  Added license that somehow went missing

  Added improved prompt keyframing, fixed image_prompts and multiple prompts

  Improved UI

  Significant under the hood cleanup and improvement

  Refined defaults for each mode

  Added latent-diffusion SuperRes for sharpening

  Added resume run mode
v4.9 Update: Feb 5th 2022 - gandamu / Adam Letts

  Added 3D

  Added brightness corrections to prevent animation from steadily going dark over time
v4.91 Update: Feb 19th 2022 - gandamu / Adam Letts

  Cleaned up 3D implementation and made associated args accessible via Colab UI elements
v4.92 Update: Feb 20th 2022 - gandamu / Adam Letts

  Separated transform code
v5.01 Update: Mar 10th 2022 - gandamu / Adam Letts

  IPython magic commands replaced by Python code
v5.1 Update: Mar 30th 2022 - zippy / Chris Allen and gandamu / Adam Letts

  Integrated Turbo+Smooth features from Disco Diffusion Turbo -- just the implementation, without its defaults.

  Implemented resume of turbo animations in such a way that it's now possible to resume from different batch folders and batch numbers.

  3D rotation parameter units are now degrees (rather than radians)

  Corrected name collision in sampling_mode (now diffusion_sampling_mode for plms/ddim, and sampling_mode for 3D transform sampling)

  Added video_init_seed_continuity option to make init video animations more continuous
v5.1 Update: Apr 4th 2022 - MSFTserver aka HostsServer

  Removed pytorch3d from needing to be compiled with a lite version specifically made for Disco Diffusion

  Remove Super Resolution

  Remove SLIP Models

  Update for crossplatform support
v5.2 Update: Apr 10th 2022 - nin_artificial / Tom Mason

  VR Mode
v5.3 Update: Jun 10th 2022 - nshepperd, huemin, cut_pow / Dmitrii Tochilkin

  Horizontal and Vertical symmetry

  Addition of ViT-L/14@336px model (requires high VRAM)
v5.4 Update: Jun 14th 2022 - devdef / Alex Spirin, Alex's Warp changes integrated into DD main by gandamu / Adam Letts

  Warp mode - for smooth/continuous video input results leveraging optical flow estimation and frame blending

  Custom models support
