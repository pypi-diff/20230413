# Comparing `tmp/samclipdiffusion-0.0.1b2.tar.gz` & `tmp/samclipdiffusion-0.0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/samclipdiffusion-0.0.1b2.tar", last modified: Tue Apr 11 12:27:30 2023, max compression
+gzip compressed data, was "dist/samclipdiffusion-0.0.3b0.tar", last modified: Thu Apr 13 20:38:09 2023, max compression
```

## Comparing `samclipdiffusion-0.0.1b2.tar` & `samclipdiffusion-0.0.3b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 eren       (501) staff       (20)        0 2023-04-11 12:27:30.793336 samclipdiffusion-0.0.1b2/
--rw-r--r--   0 eren       (501) staff       (20)     2547 2023-04-11 12:27:30.792954 samclipdiffusion-0.0.1b2/PKG-INFO
--rw-r--r--   0 eren       (501) staff       (20)     1384 2023-04-10 22:19:17.000000 samclipdiffusion-0.0.1b2/README.md
-drwxr-xr-x   0 eren       (501) staff       (20)        0 2023-04-11 12:27:30.789580 samclipdiffusion-0.0.1b2/samclipdiffusion/
--rw-r--r--   0 eren       (501) staff       (20)       67 2023-04-10 18:34:23.000000 samclipdiffusion-0.0.1b2/samclipdiffusion/__init__.py
-drwxr-xr-x   0 eren       (501) staff       (20)        0 2023-04-11 12:27:30.792313 samclipdiffusion-0.0.1b2/samclipdiffusion/guided_diffusion_pipeline/
--rw-r--r--   0 eren       (501) staff       (20)        0 2023-04-10 18:34:09.000000 samclipdiffusion-0.0.1b2/samclipdiffusion/guided_diffusion_pipeline/__init__.py
--rw-r--r--   0 eren       (501) staff       (20)     5815 2023-04-10 18:31:39.000000 samclipdiffusion-0.0.1b2/samclipdiffusion/image_segmenter.py
-drwxr-xr-x   0 eren       (501) staff       (20)        0 2023-04-11 12:27:30.791811 samclipdiffusion-0.0.1b2/samclipdiffusion.egg-info/
--rw-r--r--   0 eren       (501) staff       (20)     2547 2023-04-11 12:27:30.000000 samclipdiffusion-0.0.1b2/samclipdiffusion.egg-info/PKG-INFO
--rw-r--r--   0 eren       (501) staff       (20)      337 2023-04-11 12:27:30.000000 samclipdiffusion-0.0.1b2/samclipdiffusion.egg-info/SOURCES.txt
--rw-r--r--   0 eren       (501) staff       (20)        1 2023-04-11 12:27:30.000000 samclipdiffusion-0.0.1b2/samclipdiffusion.egg-info/dependency_links.txt
--rw-r--r--   0 eren       (501) staff       (20)       61 2023-04-11 12:27:30.000000 samclipdiffusion-0.0.1b2/samclipdiffusion.egg-info/requires.txt
--rw-r--r--   0 eren       (501) staff       (20)       17 2023-04-11 12:27:30.000000 samclipdiffusion-0.0.1b2/samclipdiffusion.egg-info/top_level.txt
--rw-r--r--   0 eren       (501) staff       (20)       38 2023-04-11 12:27:30.793546 samclipdiffusion-0.0.1b2/setup.cfg
--rw-r--r--   0 eren       (501) staff       (20)     1200 2023-04-11 12:26:55.000000 samclipdiffusion-0.0.1b2/setup.py
+drwxr-xr-x   0 eren       (501) staff       (20)        0 2023-04-13 20:38:09.459204 samclipdiffusion-0.0.3b0/
+-rw-r--r--   0 eren       (501) staff       (20)     2547 2023-04-13 20:38:09.459031 samclipdiffusion-0.0.3b0/PKG-INFO
+-rw-r--r--   0 eren       (501) staff       (20)     1384 2023-04-10 22:19:17.000000 samclipdiffusion-0.0.3b0/README.md
+drwxr-xr-x   0 eren       (501) staff       (20)        0 2023-04-13 20:38:09.457846 samclipdiffusion-0.0.3b0/samclipdiffusion/
+-rw-r--r--   0 eren       (501) staff       (20)       67 2023-04-13 20:37:36.000000 samclipdiffusion-0.0.3b0/samclipdiffusion/__init__.py
+drwxr-xr-x   0 eren       (501) staff       (20)        0 2023-04-13 20:38:09.458832 samclipdiffusion-0.0.3b0/samclipdiffusion/guided_diffusion_pipeline/
+-rw-r--r--   0 eren       (501) staff       (20)        0 2023-04-10 18:34:09.000000 samclipdiffusion-0.0.3b0/samclipdiffusion/guided_diffusion_pipeline/__init__.py
+-rw-r--r--   0 eren       (501) staff       (20)     6053 2023-04-13 19:06:06.000000 samclipdiffusion-0.0.3b0/samclipdiffusion/image_segmenter.py
+drwxr-xr-x   0 eren       (501) staff       (20)        0 2023-04-13 20:38:09.458701 samclipdiffusion-0.0.3b0/samclipdiffusion.egg-info/
+-rw-r--r--   0 eren       (501) staff       (20)     2547 2023-04-13 20:38:09.000000 samclipdiffusion-0.0.3b0/samclipdiffusion.egg-info/PKG-INFO
+-rw-r--r--   0 eren       (501) staff       (20)      337 2023-04-13 20:38:09.000000 samclipdiffusion-0.0.3b0/samclipdiffusion.egg-info/SOURCES.txt
+-rw-r--r--   0 eren       (501) staff       (20)        1 2023-04-13 20:38:09.000000 samclipdiffusion-0.0.3b0/samclipdiffusion.egg-info/dependency_links.txt
+-rw-r--r--   0 eren       (501) staff       (20)       61 2023-04-13 20:38:09.000000 samclipdiffusion-0.0.3b0/samclipdiffusion.egg-info/requires.txt
+-rw-r--r--   0 eren       (501) staff       (20)       17 2023-04-13 20:38:09.000000 samclipdiffusion-0.0.3b0/samclipdiffusion.egg-info/top_level.txt
+-rw-r--r--   0 eren       (501) staff       (20)       38 2023-04-13 20:38:09.459260 samclipdiffusion-0.0.3b0/setup.cfg
+-rw-r--r--   0 eren       (501) staff       (20)     1200 2023-04-13 20:37:32.000000 samclipdiffusion-0.0.3b0/setup.py
```

### Comparing `samclipdiffusion-0.0.1b2/PKG-INFO` & `samclipdiffusion-0.0.3b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samclipdiffusion
-Version: 0.0.1b2
+Version: 0.0.3b0
 Summary: A package for clip-guided diffusion
 Home-page: https://github.com/eren23/sam-clip-diffusion
 Author: Eren Akbulut
 Author-email: erenakbulutwork@gmail.com
 License: UNKNOWN
 Description: # SAM + CLIP + DIFFUSION
```

### Comparing `samclipdiffusion-0.0.1b2/README.md` & `samclipdiffusion-0.0.3b0/README.md`

 * *Files identical despite different names*

### Comparing `samclipdiffusion-0.0.1b2/samclipdiffusion/image_segmenter.py` & `samclipdiffusion-0.0.3b0/samclipdiffusion/image_segmenter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import cv2
 from segment_anything import build_sam, SamAutomaticMaskGenerator
 from PIL import Image, ImageDraw
 import clip
 import torch
 import numpy as np
+
+
 class ImageSegmenter:
     def __init__(self, sam_checkpoint="sam_vit_h_4b8939.pth", clip_model="ViT-B/32"):
-        self.mask_generator = SamAutomaticMaskGenerator(build_sam(checkpoint=sam_checkpoint))
+        self.mask_generator = SamAutomaticMaskGenerator(
+            build_sam(checkpoint=sam_checkpoint)
+        )
         self.clip_device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        self.clip_model, self.clip_preprocess = clip.load(clip_model, device=self.clip_device)
+        self.clip_model, self.clip_preprocess = clip.load(
+            clip_model, device=self.clip_device
+        )
 
     @staticmethod
     def convert_box_xywh_to_xyxy(box):
         x1 = box[0]
         y1 = box[1]
         x2 = box[0] + box[2]
         y2 = box[1] + box[3]
@@ -23,114 +29,134 @@
         image_array = np.array(image)
         segmented_image_array = np.zeros_like(image_array)
         segmented_image_array[segmentation_mask] = image_array[segmentation_mask]
         segmented_image = Image.fromarray(segmented_image_array)
         black_image = Image.new("RGB", image.size, (0, 0, 0))
         transparency_mask = np.zeros_like(segmentation_mask, dtype=np.uint8)
         transparency_mask[segmentation_mask] = 255
-        transparency_mask_image = Image.fromarray(transparency_mask, mode='L')
+        transparency_mask_image = Image.fromarray(transparency_mask, mode="L")
         black_image.paste(segmented_image, mask=transparency_mask_image)
         return black_image
 
     def segment_and_retrieve(self, image_path, search_text, threshold=0.05):
         # Load image
         image = Image.open(image_path)
 
         # Generate masks
         masks = self.mask_generator.generate(np.array(image))
 
         # Cut out all masks
         cropped_boxes = []
         for mask in masks:
             cropped_boxes.append(
-                self.segment_image(image, mask["segmentation"]).crop(self.convert_box_xywh_to_xyxy(mask["bbox"]))
+                self.segment_image(image, mask["segmentation"]).crop(
+                    self.convert_box_xywh_to_xyxy(mask["bbox"])
+                )
             )
 
         # Load CLIP
         model, preprocess = self.clip_model, self.clip_preprocess
 
         @torch.no_grad()
         def retriev(elements: list[Image.Image], search_text: str) -> int:
-            preprocessed_images = [preprocess(image).to(self.clip_device) for image in elements]
+            preprocessed_images = [
+                preprocess(image).to(self.clip_device) for image in elements
+            ]
             tokenized_text = clip.tokenize([search_text]).to(self.clip_device)
             stacked_images = torch.stack(preprocessed_images)
             image_features = model.encode_image(stacked_images)
             text_features = model.encode_text(tokenized_text)
             image_features /= image_features.norm(dim=-1, keepdim=True)
             text_features /= text_features.norm(dim=-1, keepdim=True)
-            probs = 100. * image_features @ text_features.T
+            probs = 100.0 * image_features @ text_features.T
             return probs[:, 0].softmax(dim=0)
 
         # Retrieve relevant images
         scores = retriev(cropped_boxes, search_text)
         indices = [i for i, v in enumerate(scores) if v > threshold]
 
         # Generate overlay image
         segmentation_masks = []
         for seg_idx in indices:
-            segmentation_mask_image = Image.fromarray(masks[seg_idx]["segmentation"].astype('uint8') * 255)
+            segmentation_mask_image = Image.fromarray(
+                masks[seg_idx]["segmentation"].astype("uint8") * 255
+            )
             segmentation_masks.append(segmentation_mask_image)
 
-        overlay_image = Image.new('RGBA', image.size, (0, 0, 0, 0))
+        overlay_image = Image.new("RGBA", image.size, (0, 0, 0, 0))
         overlay_color = (255, 0, 0, 200)
 
         draw = ImageDraw.Draw(overlay_image)
         for segmentation_mask_image in segmentation_masks:
             draw.bitmap((0, 0), segmentation_mask_image, fill=overlay_color)
         # Overlay the masks on the original image
-        result_image = Image.alpha_composite(image.convert('RGBA'), overlay_image)
-        
+        result_image = Image.alpha_composite(image.convert("RGBA"), overlay_image)
+
         return result_image, segmentation_masks
 
-    def inpaint_image(self, image_path, search_text, prompt):
+    def inpaint_image(
+        self,
+        image_path,
+        search_text,
+        prompt,
+        num_inference_steps=50,
+        negative_prompt=None,
+        guidance_scale=7.5,
+    ):
         from PIL import ImageChops, ImageFilter
         from scipy import ndimage
         from diffusers import StableDiffusionInpaintPipeline
         from functools import reduce
 
         # Load the image
         image = Image.open(image_path)
 
         # Call the segment_and_retrieve method to obtain the result image with segmentation masks
-        result_image, segmentation_masks = self.segment_and_retrieve(image_path, search_text)
-
-        # Extract the segmentation masks
-        # segmentation_masks = []
-        # for seg_idx in range(len(result_image.getbands())):
-        #     if result_image.getbands()[seg_idx] == 'A':
-        #         segmentation_masks.append(result_image.getchannel(seg_idx))
+        result_image, segmentation_masks = self.segment_and_retrieve(
+            image_path, search_text
+        )
 
         # Merge masks
         merged_mask = reduce(ImageChops.add, segmentation_masks)
         # merged_mask = ImageChops.add(segmentation_masks[0] , segmentation_masks[1])
 
         # Convert the binary mask image to a numpy array
         mask_array = np.array(merged_mask)
 
         # Define a structuring element for morphological operations
         structuring_element = ndimage.generate_binary_structure(2, 2)
 
         # Perform erosion to remove small isolated pixels
-        eroded_mask = ndimage.binary_erosion(mask_array, structure=structuring_element, iterations=2)
+        eroded_mask = ndimage.binary_erosion(
+            mask_array, structure=structuring_element, iterations=2
+        )
 
         # Perform dilation to fill small holes in the object masks
-        dilated_mask = ndimage.binary_dilation(eroded_mask, structure=structuring_element, iterations=2)
+        dilated_mask = ndimage.binary_dilation(
+            eroded_mask, structure=structuring_element, iterations=2
+        )
 
         # Convert the numpy array back to a PIL image
         filtered_mask = Image.fromarray(np.uint8(dilated_mask) * 255)
 
         image_source_for_inpaint = image.resize((512, 512))
         image_mask_for_inpaint = filtered_mask.resize((512, 512))
 
         pipe = StableDiffusionInpaintPipeline.from_pretrained(
             "stabilityai/stable-diffusion-2-inpainting",
             torch_dtype=torch.float16,
         )
 
         pipe = pipe.to("cuda")
 
-        image_inpainting = pipe(prompt=prompt, image=image_source_for_inpaint, mask_image=image_mask_for_inpaint).images[0]
+        image_inpainting = pipe(
+            prompt=prompt,
+            image=image_source_for_inpaint,
+            mask_image=image_mask_for_inpaint,
+            num_inference_steps=num_inference_steps,
+            negative_prompt=negative_prompt,
+            guidance_scale=guidance_scale,
+        ).images[0]
 
         image_inpainting = image_inpainting.resize((image.size[0], image.size[1]))
 
         return image_inpainting
-
```

### Comparing `samclipdiffusion-0.0.1b2/samclipdiffusion.egg-info/PKG-INFO` & `samclipdiffusion-0.0.3b0/samclipdiffusion.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samclipdiffusion
-Version: 0.0.1b2
+Version: 0.0.3b0
 Summary: A package for clip-guided diffusion
 Home-page: https://github.com/eren23/sam-clip-diffusion
 Author: Eren Akbulut
 Author-email: erenakbulutwork@gmail.com
 License: UNKNOWN
 Description: # SAM + CLIP + DIFFUSION
```

### Comparing `samclipdiffusion-0.0.1b2/setup.py` & `samclipdiffusion-0.0.3b0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='samclipdiffusion',
-    version='0.0.1b2',
-    description='A package for clip-guided diffusion',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    author='Eren Akbulut',
-    author_email='erenakbulutwork@gmail.com',
-    url='https://github.com/eren23/sam-clip-diffusion',
+    name="samclipdiffusion",
+    version="0.0.3b",
+    description="A package for clip-guided diffusion",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
+    author="Eren Akbulut",
+    author_email="erenakbulutwork@gmail.com",
+    url="https://github.com/eren23/sam-clip-diffusion",
     packages=find_packages(),
     install_requires=[
-        'torch',
-        'opencv-python',
-        'Pillow',
+        "torch",
+        "opencv-python",
+        "Pillow",
         # 'clip @ git+https://github.com/openai/CLIP.git',
         # 'segment_anything @ git+https://github.com/facebookresearch/segment-anything.git',
-        'diffusers',
-        'transformers',
-        'accelerate'
+        "diffusers",
+        "transformers",
+        "accelerate",
     ],
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Topic :: Scientific/Engineering :: Artificial Intelligence',
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
 )
```

