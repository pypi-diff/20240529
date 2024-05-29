# Comparing `tmp/sdkit-2.0.8.tar.gz` & `tmp/sdkit-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkit-2.0.8.tar", last modified: Wed Aug 30 13:21:10 2023, max compression
+gzip compressed data, was "sdkit-2.0.9.tar", last modified: Wed Aug 30 13:58:55 2023, max compression
```

## Comparing `sdkit-2.0.8.tar` & `sdkit-2.0.9.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:10.038613 sdkit-2.0.8/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4121 2022-12-23 10:54:05.000000 sdkit-2.0.8/LICENSE
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      140 2023-08-24 08:03:03.000000 sdkit-2.0.8/MANIFEST.in
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10710 2023-08-30 13:21:10.022982 sdkit-2.0.8/PKG-INFO
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9538 2023-08-24 08:03:03.000000 sdkit-2.0.8/README.md
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1540 2023-08-30 13:20:43.000000 sdkit-2.0.8/pyproject.toml
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:06.228976 sdkit-2.0.8/sdkit/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3803 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/__init__.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:06.511456 sdkit-2.0.8/sdkit/filter/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       41 2023-04-29 09:00:56.000000 sdkit-2.0.8/sdkit/filter/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1883 2023-08-24 07:52:49.000000 sdkit-2.0.8/sdkit/filter/apply_filters.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:06.619809 sdkit-2.0.8/sdkit/filter/codeformer/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4584 2023-06-12 10:09:16.000000 sdkit-2.0.8/sdkit/filter/codeformer/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    25361 2023-06-01 09:41:33.000000 sdkit-2.0.8/sdkit/filter/codeformer/face_restoration_helper.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     7317 2023-06-01 09:41:35.000000 sdkit-2.0.8/sdkit/filter/codeformer/misc.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      998 2023-02-16 16:25:27.000000 sdkit-2.0.8/sdkit/filter/gfpgan.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      514 2023-08-24 07:53:59.000000 sdkit-2.0.8/sdkit/filter/latent_upscaler.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      614 2023-04-28 10:50:58.000000 sdkit-2.0.8/sdkit/filter/nsfw_checker.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      378 2023-04-10 12:49:03.000000 sdkit-2.0.8/sdkit/filter/realesrgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:06.698336 sdkit-2.0.8/sdkit/generate/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       45 2023-04-29 09:01:13.000000 sdkit-2.0.8/sdkit/generate/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    19289 2023-08-30 11:10:38.000000 sdkit-2.0.8/sdkit/generate/image_generator.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2479 2023-02-17 07:20:50.000000 sdkit-2.0.8/sdkit/generate/prompt_parser.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:06.917917 sdkit-2.0.8/sdkit/generate/sampler/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:07.000000 sdkit-2.0.8/sdkit/generate/sampler/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3168 2023-04-10 11:16:32.000000 sdkit-2.0.8/sdkit/generate/sampler/default_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3967 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/generate/sampler/diffusers_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2589 2023-02-16 16:25:27.000000 sdkit-2.0.8/sdkit/generate/sampler/k_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2132 2023-02-16 16:27:22.000000 sdkit-2.0.8/sdkit/generate/sampler/sampler_main.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:07.014084 sdkit-2.0.8/sdkit/generate/sampler/unipc_samplers/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2737 2023-07-24 06:36:08.000000 sdkit-2.0.8/sdkit/generate/sampler/unipc_samplers/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    40444 2023-04-29 08:59:42.000000 sdkit-2.0.8/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:07.121884 sdkit-2.0.8/sdkit/models/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      258 2023-07-06 13:00:18.000000 sdkit-2.0.8/sdkit/models/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     5637 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/model_downloader.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:07.545383 sdkit-2.0.8/sdkit/models/model_loader/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2839 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/model_loader/__init__.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:07.687980 sdkit-2.0.8/sdkit/models/model_loader/codeformer/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      560 2023-05-30 11:07:00.000000 sdkit-2.0.8/sdkit/models/model_loader/codeformer/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11004 2023-05-30 11:06:45.000000 sdkit-2.0.8/sdkit/models/model_loader/codeformer/codeformer_arch.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    15271 2023-05-30 11:06:54.000000 sdkit-2.0.8/sdkit/models/model_loader/codeformer/vqgan_arch.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2627 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/model_loader/controlnet.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1232 2023-08-24 07:43:53.000000 sdkit-2.0.8/sdkit/models/model_loader/controlnet_filters.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    31461 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/model_loader/diffusers_bugfixes.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4071 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/model_loader/embeddings.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      609 2023-02-16 16:25:27.000000 sdkit-2.0.8/sdkit/models/model_loader/gfpgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:07.782144 sdkit-2.0.8/sdkit/models/model_loader/hypernetwork/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2337 2023-02-16 16:25:27.000000 sdkit-2.0.8/sdkit/models/model_loader/hypernetwork/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4414 2023-02-16 16:25:27.000000 sdkit-2.0.8/sdkit/models/model_loader/hypernetwork/hypernetwork.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      738 2023-06-23 16:10:08.000000 sdkit-2.0.8/sdkit/models/model_loader/latent_upscaler.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10842 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/model_loader/lora.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      609 2023-06-05 10:16:25.000000 sdkit-2.0.8/sdkit/models/model_loader/nsfw_checker.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1117 2023-04-20 10:42:08.000000 sdkit-2.0.8/sdkit/models/model_loader/realesrgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:07.907585 sdkit-2.0.8/sdkit/models/model_loader/stable_diffusion/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    22159 2023-08-30 12:51:29.000000 sdkit-2.0.8/sdkit/models/model_loader/stable_diffusion/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    14464 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/model_loader/stable_diffusion/accelerators.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10003 2023-07-31 05:22:01.000000 sdkit-2.0.8/sdkit/models/model_loader/stable_diffusion/optimizations.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3043 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/model_loader/vae.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:08.177661 sdkit-2.0.8/sdkit/models/models_db/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1352 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/models_db/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      256 2023-05-29 11:06:44.000000 sdkit-2.0.8/sdkit/models/models_db/codeformer.json
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:08.696086 sdkit-2.0.8/sdkit/models/models_db/configs/
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:09.380211 sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1982 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11e_sd15_shuffle.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11f1e_sd15_tile.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11f1p_sd15_depth.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_canny.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_inpaint.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_lineart.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_mlsd.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_normalbae.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_openpose.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_scribble.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_seg.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_softedge.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15s2_lineart_anime.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3247 2023-08-24 07:43:53.000000 sdkit-2.0.8/sdkit/models/models_db/configs/sd-xl-base-1.0.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2948 2023-08-24 07:43:53.000000 sdkit-2.0.8/sdkit/models/models_db/configs/sd-xl-refiner-1.0.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1873 2022-12-25 10:25:54.000000 sdkit-2.0.8/sdkit/models/models_db/configs/v1-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1991 2022-12-25 10:26:03.000000 sdkit-2.0.8/sdkit/models/models_db/configs/v1-inpainting-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1815 2022-12-25 10:26:48.000000 sdkit-2.0.8/sdkit/models/models_db/configs/v2-inference-v.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1789 2022-12-25 10:26:58.000000 sdkit-2.0.8/sdkit/models/models_db/configs/v2-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4450 2022-12-25 10:26:26.000000 sdkit-2.0.8/sdkit/models/models_db/configs/v2-inpainting-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1869 2022-12-25 10:26:35.000000 sdkit-2.0.8/sdkit/models/models_db/configs/v2-midas-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1847 2023-06-20 05:11:27.000000 sdkit-2.0.8/sdkit/models/models_db/configs/v2.1-inference-v.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1821 2023-08-22 07:02:04.000000 sdkit-2.0.8/sdkit/models/models_db/configs/v2.1-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2251 2022-12-25 10:26:13.000000 sdkit-2.0.8/sdkit/models/models_db/configs/x4-upscaling.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4501 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/models/models_db/controlnet.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      720 2023-04-22 10:11:26.000000 sdkit-2.0.8/sdkit/models/models_db/gfpgan.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      534 2023-05-29 11:07:36.000000 sdkit-2.0.8/sdkit/models/models_db/realesrgan.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11274 2023-08-29 14:30:58.000000 sdkit-2.0.8/sdkit/models/models_db/stable_diffusion.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      308 2023-04-19 09:15:54.000000 sdkit-2.0.8/sdkit/models/models_db/vae.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      206 2023-02-16 16:25:27.000000 sdkit-2.0.8/sdkit/models/scan_models.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:09.442720 sdkit-2.0.8/sdkit/train/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       62 2023-07-31 05:22:01.000000 sdkit-2.0.8/sdkit/train/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4509 2023-07-31 05:22:01.000000 sdkit-2.0.8/sdkit/train/merge_models.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:09.756003 sdkit-2.0.8/sdkit/utils/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1226 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/utils/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    12288 2023-08-30 13:18:12.000000 sdkit-2.0.8/sdkit/utils/convert_model_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      595 2023-07-08 13:04:53.000000 sdkit-2.0.8/sdkit/utils/device_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4137 2023-07-31 05:22:01.000000 sdkit-2.0.8/sdkit/utils/file_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2192 2023-07-06 14:00:45.000000 sdkit-2.0.8/sdkit/utils/hash_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1116 2023-07-06 14:00:45.000000 sdkit-2.0.8/sdkit/utils/http_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2916 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/utils/image_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4938 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/utils/latent_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     6929 2023-07-06 14:00:45.000000 sdkit-2.0.8/sdkit/utils/memory_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1239 2023-08-24 08:03:03.000000 sdkit-2.0.8/sdkit/utils/misc_utils.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:06.338772 sdkit-2.0.8/sdkit.egg-info/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10710 2023-08-30 13:21:04.000000 sdkit-2.0.8/sdkit.egg-info/PKG-INFO
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4269 2023-08-30 13:21:05.000000 sdkit-2.0.8/sdkit.egg-info/SOURCES.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        1 2023-08-30 13:21:04.000000 sdkit-2.0.8/sdkit.egg-info/dependency_links.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      206 2023-08-30 13:21:04.000000 sdkit-2.0.8/sdkit.egg-info/requires.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        6 2023-08-30 13:21:04.000000 sdkit-2.0.8/sdkit.egg-info/top_level.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       38 2023-08-30 13:21:10.038613 sdkit-2.0.8/setup.cfg
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      497 2023-08-29 03:48:19.000000 sdkit-2.0.8/setup.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:21:10.007375 sdkit-2.0.8/tests/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1643 2023-06-12 12:36:25.000000 sdkit-2.0.8/tests/test_codeformer.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    12435 2023-08-24 07:52:49.000000 sdkit-2.0.8/tests/test_controlnet.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1552 2023-08-02 14:30:53.000000 sdkit-2.0.8/tests/test_directml_tensorrt.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     5827 2023-08-24 08:03:03.000000 sdkit-2.0.8/tests/test_embeddings.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1415 2023-08-24 07:52:49.000000 sdkit-2.0.8/tests/test_gfpgan_realesrgan.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     7489 2023-08-24 08:03:03.000000 sdkit-2.0.8/tests/test_lora.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3628 2023-07-31 05:22:01.000000 sdkit-2.0.8/tests/test_model_merge.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     8970 2023-08-29 14:33:48.000000 sdkit-2.0.8/tests/test_stable_diffusion_detailed.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    13724 2023-08-29 14:33:55.000000 sdkit-2.0.8/tests/test_stable_diffusion_quick.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1171 2023-08-24 08:10:33.000000 sdkit-2.0.8/tests/test_tiling.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:55.833804 sdkit-2.0.9/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4121 2022-12-23 10:54:05.000000 sdkit-2.0.9/LICENSE
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      140 2023-08-24 08:03:03.000000 sdkit-2.0.9/MANIFEST.in
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10710 2023-08-30 13:58:55.833804 sdkit-2.0.9/PKG-INFO
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9538 2023-08-24 08:03:03.000000 sdkit-2.0.9/README.md
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1540 2023-08-30 13:58:26.000000 sdkit-2.0.9/pyproject.toml
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:52.155172 sdkit-2.0.9/sdkit/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3803 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/__init__.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:52.410128 sdkit-2.0.9/sdkit/filter/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       41 2023-04-29 09:00:56.000000 sdkit-2.0.9/sdkit/filter/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1883 2023-08-24 07:52:49.000000 sdkit-2.0.9/sdkit/filter/apply_filters.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:52.512666 sdkit-2.0.9/sdkit/filter/codeformer/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4584 2023-06-12 10:09:16.000000 sdkit-2.0.9/sdkit/filter/codeformer/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    25361 2023-06-01 09:41:33.000000 sdkit-2.0.9/sdkit/filter/codeformer/face_restoration_helper.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     7317 2023-06-01 09:41:35.000000 sdkit-2.0.9/sdkit/filter/codeformer/misc.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      998 2023-02-16 16:25:27.000000 sdkit-2.0.9/sdkit/filter/gfpgan.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      514 2023-08-24 07:53:59.000000 sdkit-2.0.9/sdkit/filter/latent_upscaler.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      614 2023-04-28 10:50:58.000000 sdkit-2.0.9/sdkit/filter/nsfw_checker.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      378 2023-04-10 12:49:03.000000 sdkit-2.0.9/sdkit/filter/realesrgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:52.592843 sdkit-2.0.9/sdkit/generate/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       45 2023-04-29 09:01:13.000000 sdkit-2.0.9/sdkit/generate/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    19289 2023-08-30 11:10:38.000000 sdkit-2.0.9/sdkit/generate/image_generator.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2479 2023-02-17 07:20:50.000000 sdkit-2.0.9/sdkit/generate/prompt_parser.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:52.749519 sdkit-2.0.9/sdkit/generate/sampler/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:07.000000 sdkit-2.0.9/sdkit/generate/sampler/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3168 2023-04-10 11:16:32.000000 sdkit-2.0.9/sdkit/generate/sampler/default_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3967 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/generate/sampler/diffusers_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2589 2023-02-16 16:25:27.000000 sdkit-2.0.9/sdkit/generate/sampler/k_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2132 2023-02-16 16:27:22.000000 sdkit-2.0.9/sdkit/generate/sampler/sampler_main.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:52.838442 sdkit-2.0.9/sdkit/generate/sampler/unipc_samplers/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2737 2023-07-24 06:36:08.000000 sdkit-2.0.9/sdkit/generate/sampler/unipc_samplers/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    40444 2023-04-29 08:59:42.000000 sdkit-2.0.9/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:52.923374 sdkit-2.0.9/sdkit/models/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      258 2023-07-06 13:00:18.000000 sdkit-2.0.9/sdkit/models/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     5637 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/model_downloader.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:53.324815 sdkit-2.0.9/sdkit/models/model_loader/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2839 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/model_loader/__init__.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:53.471897 sdkit-2.0.9/sdkit/models/model_loader/codeformer/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      560 2023-05-30 11:07:00.000000 sdkit-2.0.9/sdkit/models/model_loader/codeformer/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11004 2023-05-30 11:06:45.000000 sdkit-2.0.9/sdkit/models/model_loader/codeformer/codeformer_arch.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    15271 2023-05-30 11:06:54.000000 sdkit-2.0.9/sdkit/models/model_loader/codeformer/vqgan_arch.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2627 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/model_loader/controlnet.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1232 2023-08-24 07:43:53.000000 sdkit-2.0.9/sdkit/models/model_loader/controlnet_filters.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    31461 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/model_loader/diffusers_bugfixes.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4071 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/model_loader/embeddings.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      609 2023-02-16 16:25:27.000000 sdkit-2.0.9/sdkit/models/model_loader/gfpgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:53.570116 sdkit-2.0.9/sdkit/models/model_loader/hypernetwork/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2337 2023-02-16 16:25:27.000000 sdkit-2.0.9/sdkit/models/model_loader/hypernetwork/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4414 2023-02-16 16:25:27.000000 sdkit-2.0.9/sdkit/models/model_loader/hypernetwork/hypernetwork.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      738 2023-06-23 16:10:08.000000 sdkit-2.0.9/sdkit/models/model_loader/latent_upscaler.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10842 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/model_loader/lora.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      609 2023-06-05 10:16:25.000000 sdkit-2.0.9/sdkit/models/model_loader/nsfw_checker.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1117 2023-04-20 10:42:08.000000 sdkit-2.0.9/sdkit/models/model_loader/realesrgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:53.713362 sdkit-2.0.9/sdkit/models/model_loader/stable_diffusion/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    22728 2023-08-30 13:49:02.000000 sdkit-2.0.9/sdkit/models/model_loader/stable_diffusion/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    14464 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/model_loader/stable_diffusion/accelerators.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10003 2023-07-31 05:22:01.000000 sdkit-2.0.9/sdkit/models/model_loader/stable_diffusion/optimizations.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3043 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/model_loader/vae.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:53.982517 sdkit-2.0.9/sdkit/models/models_db/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1352 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/models_db/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      256 2023-05-29 11:06:44.000000 sdkit-2.0.9/sdkit/models/models_db/codeformer.json
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:54.492830 sdkit-2.0.9/sdkit/models/models_db/configs/
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:55.183074 sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1982 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11e_sd15_shuffle.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11f1e_sd15_tile.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11f1p_sd15_depth.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_canny.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_inpaint.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_lineart.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_mlsd.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_normalbae.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_openpose.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_scribble.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_seg.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_softedge.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1949 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15s2_lineart_anime.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3247 2023-08-24 07:43:53.000000 sdkit-2.0.9/sdkit/models/models_db/configs/sd-xl-base-1.0.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2948 2023-08-24 07:43:53.000000 sdkit-2.0.9/sdkit/models/models_db/configs/sd-xl-refiner-1.0.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1873 2022-12-25 10:25:54.000000 sdkit-2.0.9/sdkit/models/models_db/configs/v1-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1991 2022-12-25 10:26:03.000000 sdkit-2.0.9/sdkit/models/models_db/configs/v1-inpainting-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1815 2022-12-25 10:26:48.000000 sdkit-2.0.9/sdkit/models/models_db/configs/v2-inference-v.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1789 2022-12-25 10:26:58.000000 sdkit-2.0.9/sdkit/models/models_db/configs/v2-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4450 2022-12-25 10:26:26.000000 sdkit-2.0.9/sdkit/models/models_db/configs/v2-inpainting-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1869 2022-12-25 10:26:35.000000 sdkit-2.0.9/sdkit/models/models_db/configs/v2-midas-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1847 2023-06-20 05:11:27.000000 sdkit-2.0.9/sdkit/models/models_db/configs/v2.1-inference-v.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1821 2023-08-22 07:02:04.000000 sdkit-2.0.9/sdkit/models/models_db/configs/v2.1-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2251 2022-12-25 10:26:13.000000 sdkit-2.0.9/sdkit/models/models_db/configs/x4-upscaling.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4501 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/models/models_db/controlnet.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      720 2023-04-22 10:11:26.000000 sdkit-2.0.9/sdkit/models/models_db/gfpgan.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      534 2023-05-29 11:07:36.000000 sdkit-2.0.9/sdkit/models/models_db/realesrgan.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11274 2023-08-29 14:30:58.000000 sdkit-2.0.9/sdkit/models/models_db/stable_diffusion.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      308 2023-04-19 09:15:54.000000 sdkit-2.0.9/sdkit/models/models_db/vae.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      206 2023-02-16 16:25:27.000000 sdkit-2.0.9/sdkit/models/scan_models.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:55.250517 sdkit-2.0.9/sdkit/train/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       62 2023-07-31 05:22:01.000000 sdkit-2.0.9/sdkit/train/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4509 2023-07-31 05:22:01.000000 sdkit-2.0.9/sdkit/train/merge_models.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:55.538000 sdkit-2.0.9/sdkit/utils/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1226 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/utils/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11906 2023-08-30 13:49:18.000000 sdkit-2.0.9/sdkit/utils/convert_model_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      595 2023-07-08 13:04:53.000000 sdkit-2.0.9/sdkit/utils/device_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4137 2023-07-31 05:22:01.000000 sdkit-2.0.9/sdkit/utils/file_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2192 2023-07-06 14:00:45.000000 sdkit-2.0.9/sdkit/utils/hash_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1116 2023-07-06 14:00:45.000000 sdkit-2.0.9/sdkit/utils/http_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2916 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/utils/image_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4938 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/utils/latent_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     6929 2023-07-06 14:00:45.000000 sdkit-2.0.9/sdkit/utils/memory_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1239 2023-08-24 08:03:03.000000 sdkit-2.0.9/sdkit/utils/misc_utils.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:52.249349 sdkit-2.0.9/sdkit.egg-info/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10710 2023-08-30 13:58:50.000000 sdkit-2.0.9/sdkit.egg-info/PKG-INFO
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4269 2023-08-30 13:58:51.000000 sdkit-2.0.9/sdkit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        1 2023-08-30 13:58:50.000000 sdkit-2.0.9/sdkit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      206 2023-08-30 13:58:50.000000 sdkit-2.0.9/sdkit.egg-info/requires.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        6 2023-08-30 13:58:50.000000 sdkit-2.0.9/sdkit.egg-info/top_level.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       38 2023-08-30 13:58:55.833804 sdkit-2.0.9/setup.cfg
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      497 2023-08-29 03:48:19.000000 sdkit-2.0.9/setup.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-08-30 13:58:55.805484 sdkit-2.0.9/tests/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1643 2023-06-12 12:36:25.000000 sdkit-2.0.9/tests/test_codeformer.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    12435 2023-08-24 07:52:49.000000 sdkit-2.0.9/tests/test_controlnet.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1552 2023-08-02 14:30:53.000000 sdkit-2.0.9/tests/test_directml_tensorrt.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     5827 2023-08-24 08:03:03.000000 sdkit-2.0.9/tests/test_embeddings.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1415 2023-08-24 07:52:49.000000 sdkit-2.0.9/tests/test_gfpgan_realesrgan.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     7489 2023-08-24 08:03:03.000000 sdkit-2.0.9/tests/test_lora.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3628 2023-07-31 05:22:01.000000 sdkit-2.0.9/tests/test_model_merge.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     8970 2023-08-29 14:33:48.000000 sdkit-2.0.9/tests/test_stable_diffusion_detailed.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    13724 2023-08-29 14:33:55.000000 sdkit-2.0.9/tests/test_stable_diffusion_quick.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1171 2023-08-24 08:10:33.000000 sdkit-2.0.9/tests/test_tiling.py
```

### Comparing `sdkit-2.0.8/LICENSE` & `sdkit-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/PKG-INFO` & `sdkit-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkit
-Version: 2.0.8
+Version: 2.0.9
 Summary: sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like SDXL, ControlNet, LoRA, Embeddings, GFPGAN, RealESRGAN, k-samplers, custom VAE etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc.
 Author-email: cmdr2 <secondary.cmdr2@gmail.com>
 Project-URL: Homepage, https://github.com/easydiffusion/sdkit
 Project-URL: Bug Tracker, https://github.com/easydiffusion/sdkit/issues
 Keywords: stable diffusion,ai,art
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkit-2.0.8/README.md` & `sdkit-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/pyproject.toml` & `sdkit-2.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sdkit"
-version = "2.0.8"
+version = "2.0.9"
 authors = [
   {name="cmdr2", email="secondary.cmdr2@gmail.com"},
 ]
 description = "sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like SDXL, ControlNet, LoRA, Embeddings, GFPGAN, RealESRGAN, k-samplers, custom VAE etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc."
 readme = "README.md"
 requires-python = ">=3.8.5"
 classifiers = [
```

### Comparing `sdkit-2.0.8/sdkit/__init__.py` & `sdkit-2.0.9/sdkit/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/filter/apply_filters.py` & `sdkit-2.0.9/sdkit/filter/apply_filters.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/filter/codeformer/__init__.py` & `sdkit-2.0.9/sdkit/filter/codeformer/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/filter/codeformer/face_restoration_helper.py` & `sdkit-2.0.9/sdkit/filter/codeformer/face_restoration_helper.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/filter/codeformer/misc.py` & `sdkit-2.0.9/sdkit/filter/codeformer/misc.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/filter/gfpgan.py` & `sdkit-2.0.9/sdkit/filter/gfpgan.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/filter/latent_upscaler.py` & `sdkit-2.0.9/sdkit/filter/latent_upscaler.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/filter/nsfw_checker.py` & `sdkit-2.0.9/sdkit/filter/nsfw_checker.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/generate/image_generator.py` & `sdkit-2.0.9/sdkit/generate/image_generator.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/generate/prompt_parser.py` & `sdkit-2.0.9/sdkit/generate/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/generate/sampler/default_samplers.py` & `sdkit-2.0.9/sdkit/generate/sampler/default_samplers.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/generate/sampler/diffusers_samplers.py` & `sdkit-2.0.9/sdkit/generate/sampler/diffusers_samplers.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/generate/sampler/k_samplers.py` & `sdkit-2.0.9/sdkit/generate/sampler/k_samplers.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/generate/sampler/sampler_main.py` & `sdkit-2.0.9/sdkit/generate/sampler/sampler_main.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/generate/sampler/unipc_samplers/__init__.py` & `sdkit-2.0.9/sdkit/generate/sampler/unipc_samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py` & `sdkit-2.0.9/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_downloader.py` & `sdkit-2.0.9/sdkit/models/model_downloader.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/__init__.py` & `sdkit-2.0.9/sdkit/models/model_loader/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/codeformer/__init__.py` & `sdkit-2.0.9/sdkit/models/model_loader/codeformer/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/codeformer/codeformer_arch.py` & `sdkit-2.0.9/sdkit/models/model_loader/codeformer/codeformer_arch.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/codeformer/vqgan_arch.py` & `sdkit-2.0.9/sdkit/models/model_loader/codeformer/vqgan_arch.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/controlnet.py` & `sdkit-2.0.9/sdkit/models/model_loader/controlnet.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/controlnet_filters.py` & `sdkit-2.0.9/sdkit/models/model_loader/controlnet_filters.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/diffusers_bugfixes.py` & `sdkit-2.0.9/sdkit/models/model_loader/diffusers_bugfixes.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/embeddings.py` & `sdkit-2.0.9/sdkit/models/model_loader/embeddings.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/gfpgan.py` & `sdkit-2.0.9/sdkit/models/model_loader/gfpgan.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/hypernetwork/__init__.py` & `sdkit-2.0.9/sdkit/models/model_loader/hypernetwork/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/hypernetwork/hypernetwork.py` & `sdkit-2.0.9/sdkit/models/model_loader/hypernetwork/hypernetwork.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/latent_upscaler.py` & `sdkit-2.0.9/sdkit/models/model_loader/latent_upscaler.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/lora.py` & `sdkit-2.0.9/sdkit/models/model_loader/lora.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/nsfw_checker.py` & `sdkit-2.0.9/sdkit/models/model_loader/nsfw_checker.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/realesrgan.py` & `sdkit-2.0.9/sdkit/models/model_loader/realesrgan.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/stable_diffusion/__init__.py` & `sdkit-2.0.9/sdkit/models/model_loader/stable_diffusion/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,15 @@
     )
     from diffusers.models.attention_processor import Attention
     from compel import Compel, DiffusersTextualInversionManager, ReturnedEmbeddingsType as Skip
     import platform
 
     from sdkit.generate.sampler import diffusers_samplers
     from sdkit.utils import gc, has_amd_gpu
+    import torch.nn.functional as F
 
     from diffusers.pipelines.stable_diffusion.convert_from_ckpt import download_from_original_stable_diffusion_ckpt
 
     log.info("loading on diffusers")
 
     log.info(f"using config: {config_file_path}")
     config = OmegaConf.load(config_file_path)
@@ -204,17 +205,45 @@
         model_load_params["pipeline_class"] = StableDiffusionInpaintPipeline
     elif is_sd_xl:
         if config.model.params.network_config.params.context_dim == 2048:
             model_load_params["pipeline_class"] = StableDiffusionXLPipeline
         else:
             model_load_params["pipeline_class"] = StableDiffusionXLImg2ImgPipeline
 
+    # optimize for TRT or DirectML (AMD on Windows)
+    model_component, _ = os.path.splitext(model_path)
+    model_trt_path = model_component + ".trt"
+    unet_onnx_path = model_component + ".unet.onnx"
+
+    use_directml = platform.system() == "Windows" and has_amd_gpu()
+    try:
+        from importlib.metadata import version
+
+        version("onnxruntime-directml")  # check if this is installed
+    except:
+        use_directml = False
+
+    if "cuda" not in context.device:
+        convert_to_tensorrt = False
+
+    # remove SDPA if torch 2.0 and need to convert to ONNX
+    needs_onnx = convert_to_tensorrt or (
+        use_directml and (not os.path.exists(unet_onnx_path) or os.stat(unet_onnx_path).st_size == 0)
+    )
+    swap_sdpa = needs_onnx and hasattr(F, "scaled_dot_product_attention")
+    old_sdpa = getattr(F, "scaled_dot_product_attention", None) if swap_sdpa else None
+    if swap_sdpa:
+        delattr(F, "scaled_dot_product_attention")
+
     # txt2img
     default_pipe = download_from_original_stable_diffusion_ckpt(state_dict, **model_load_params)
 
+    if swap_sdpa and old_sdpa:
+        setattr(F, "scaled_dot_product_attention", old_sdpa)
+
     default_pipe.requires_safety_checker = False
     default_pipe.safety_checker = None
 
     model_type = "SD1"
     if is_sd_xl:
         model_type = "SDXL"
     else:
@@ -224,30 +253,14 @@
         elif context_dim == 1024:
             model_type = "SD2"
 
     if is_sd_xl:
         # until the image artifacts go away: https://huggingface.co/stabilityai/stable-diffusion-xl-base-0.9/discussions/31
         default_pipe.watermark.apply_watermark = lambda images: images
 
-    # optimize for TRT or DirectML (AMD on Windows)
-    model_component, _ = os.path.splitext(model_path)
-    model_trt_path = model_component + ".trt"
-    unet_onnx_path = model_component + ".unet.onnx"
-
-    use_directml = platform.system() == "Windows" and has_amd_gpu()
-    try:
-        from importlib.metadata import version
-
-        version("onnxruntime-directml")  # check if this is installed
-    except:
-        use_directml = False
-
-    if "cuda" not in context.device:
-        convert_to_tensorrt = False
-
     if use_directml and (not os.path.exists(unet_onnx_path) or os.stat(unet_onnx_path).st_size == 0):
         from sdkit.utils import gc, convert_pipeline_unet_to_onnx
 
         log.info("Converting UNet to ONNX to run on AMD on Windows..")
         convert_pipeline_unet_to_onnx(default_pipe, unet_onnx_path, device="cpu", fp16=False)  # on cpu, so fp32
         log.info("Converted UNet to ONNX to run on AMD on Windows!")
     elif convert_to_tensorrt:
```

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/stable_diffusion/accelerators.py` & `sdkit-2.0.9/sdkit/models/model_loader/stable_diffusion/accelerators.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/stable_diffusion/optimizations.py` & `sdkit-2.0.9/sdkit/models/model_loader/stable_diffusion/optimizations.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/model_loader/vae.py` & `sdkit-2.0.9/sdkit/models/model_loader/vae.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/__init__.py` & `sdkit-2.0.9/sdkit/models/models_db/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11e_sd15_shuffle.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11e_sd15_shuffle.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11f1e_sd15_tile.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11f1e_sd15_tile.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11f1p_sd15_depth.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11f1p_sd15_depth.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_canny.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_canny.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_inpaint.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_inpaint.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_lineart.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_lineart.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_mlsd.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_mlsd.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_normalbae.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_normalbae.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_openpose.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_openpose.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_scribble.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_scribble.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_seg.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_seg.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_softedge.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15_softedge.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/controlnet/control_v11p_sd15s2_lineart_anime.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/controlnet/control_v11p_sd15s2_lineart_anime.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/sd-xl-base-1.0.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/sd-xl-base-1.0.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/sd-xl-refiner-1.0.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/sd-xl-refiner-1.0.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/v1-inference.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/v1-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/v1-inpainting-inference.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/v1-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/v2-inference-v.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/v2-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/v2-inference.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/v2-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/v2-inpainting-inference.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/v2-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/v2-midas-inference.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/v2-midas-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/v2.1-inference-v.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/v2.1-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/v2.1-inference.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/v2.1-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/configs/x4-upscaling.yaml` & `sdkit-2.0.9/sdkit/models/models_db/configs/x4-upscaling.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/controlnet.json` & `sdkit-2.0.9/sdkit/models/models_db/controlnet.json`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/gfpgan.json` & `sdkit-2.0.9/sdkit/models/models_db/gfpgan.json`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/realesrgan.json` & `sdkit-2.0.9/sdkit/models/models_db/realesrgan.json`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/models/models_db/stable_diffusion.json` & `sdkit-2.0.9/sdkit/models/models_db/stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/train/merge_models.py` & `sdkit-2.0.9/sdkit/train/merge_models.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/utils/__init__.py` & `sdkit-2.0.9/sdkit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/utils/convert_model_utils.py` & `sdkit-2.0.9/sdkit/utils/convert_model_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,48 +120,38 @@
     model_path = os.path.join(tmp_dir, "model.onnx") if use_external_data_format else save_path
 
     model_name, _ = os.path.splitext(save_path)
     model_name = os.path.basename(model_name)
 
     model_args = tuple(m.to(device=_device, dtype=_dtype) for m in model_args if isinstance(m, torch.Tensor))
 
-    import torch.nn.functional as F
-
-    sdpa = getattr(F, "scaled_dot_product_attention", None)
-    try:
-        if sdpa is not None:
-            delattr(F, "scaled_dot_product_attention")
-
-        onnx_export(
+    onnx_export(
+        model,
+        model_args=model_args,
+        output_path=model_path,
+        ordered_input_names=input_names,
+        output_names=["out_sample"],  # has to be different from "sample" for correct tracing
+        dynamic_axes=dynamic_axes,
+        opset=opset,
+        use_external_data_format=use_external_data_format,
+    )
+
+    if use_external_data_format:
+        model = onnx.load(model_path)
+        shutil.rmtree(tmp_dir)
+        # collate external tensor files into one
+        onnx.save_model(
             model,
-            model_args=model_args,
-            output_path=model_path,
-            ordered_input_names=input_names,
-            output_names=["out_sample"],  # has to be different from "sample" for correct tracing
-            dynamic_axes=dynamic_axes,
-            opset=opset,
-            use_external_data_format=use_external_data_format,
+            save_path,
+            save_as_external_data=use_external_data_format,
+            all_tensors_to_one_file=True,
+            location=model_name + ".onnx_weights.pb",
+            convert_attribute=False,
         )
 
-        if use_external_data_format:
-            model = onnx.load(model_path)
-            shutil.rmtree(tmp_dir)
-            # collate external tensor files into one
-            onnx.save_model(
-                model,
-                save_path,
-                save_as_external_data=use_external_data_format,
-                all_tensors_to_one_file=True,
-                location=model_name + ".onnx_weights.pb",
-                convert_attribute=False,
-            )
-    finally:
-        if sdpa is not None:
-            setattr(F, "scaled_dot_product_attention", sdpa)
-
     pipeline = pipeline.to(orig_device, torch_dtype=orig_dtype)
 
 
 def onnx_export(
     model,
     model_args: tuple,
     output_path,
```

### Comparing `sdkit-2.0.8/sdkit/utils/device_utils.py` & `sdkit-2.0.9/sdkit/utils/device_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/utils/file_utils.py` & `sdkit-2.0.9/sdkit/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/utils/hash_utils.py` & `sdkit-2.0.9/sdkit/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/utils/http_utils.py` & `sdkit-2.0.9/sdkit/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/utils/image_utils.py` & `sdkit-2.0.9/sdkit/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/utils/latent_utils.py` & `sdkit-2.0.9/sdkit/utils/latent_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/utils/memory_utils.py` & `sdkit-2.0.9/sdkit/utils/memory_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit/utils/misc_utils.py` & `sdkit-2.0.9/sdkit/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/sdkit.egg-info/PKG-INFO` & `sdkit-2.0.9/sdkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkit
-Version: 2.0.8
+Version: 2.0.9
 Summary: sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like SDXL, ControlNet, LoRA, Embeddings, GFPGAN, RealESRGAN, k-samplers, custom VAE etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc.
 Author-email: cmdr2 <secondary.cmdr2@gmail.com>
 Project-URL: Homepage, https://github.com/easydiffusion/sdkit
 Project-URL: Bug Tracker, https://github.com/easydiffusion/sdkit/issues
 Keywords: stable diffusion,ai,art
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkit-2.0.8/sdkit.egg-info/SOURCES.txt` & `sdkit-2.0.9/sdkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/tests/test_codeformer.py` & `sdkit-2.0.9/tests/test_codeformer.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/tests/test_controlnet.py` & `sdkit-2.0.9/tests/test_controlnet.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/tests/test_directml_tensorrt.py` & `sdkit-2.0.9/tests/test_directml_tensorrt.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/tests/test_embeddings.py` & `sdkit-2.0.9/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/tests/test_gfpgan_realesrgan.py` & `sdkit-2.0.9/tests/test_gfpgan_realesrgan.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/tests/test_lora.py` & `sdkit-2.0.9/tests/test_lora.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/tests/test_model_merge.py` & `sdkit-2.0.9/tests/test_model_merge.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/tests/test_stable_diffusion_detailed.py` & `sdkit-2.0.9/tests/test_stable_diffusion_detailed.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/tests/test_stable_diffusion_quick.py` & `sdkit-2.0.9/tests/test_stable_diffusion_quick.py`

 * *Files identical despite different names*

### Comparing `sdkit-2.0.8/tests/test_tiling.py` & `sdkit-2.0.9/tests/test_tiling.py`

 * *Files identical despite different names*

