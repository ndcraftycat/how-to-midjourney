# **Join the Midjourney Discord Server**

You'll need a Discord account to use Midjourney. Once you're logged in, join the Midjourney server, or invite the bot to your private server. 

[Midjourney Discord Interface](https://docs.midjourney.com/docs/midjourney-discord)

# **Interact with the Midjourney Bot**

You can access the Midjourney Bot anywhere on Discord. Use the bot to generate images based on your text prompts. 

this is the full command list:

[Midjourney Command List](https://docs.midjourney.com/docs/command-list)

**Noteworthy commands:**

1. Use the **`/info`** command to see information about your current queued and running jobs, subscription type, renewal date, and more.
2. **`/subscribe`** - Generate a personal link for a user's account page. 
also see: [https://www.midjourney.com/account/](https://www.midjourney.com/account/) 
all about subscriptions: [https://docs.midjourney.com/docs/plans](https://docs.midjourney.com/docs/plans)
3. The **`/settings`** command provides toggle buttons for common options like model version, style value, quality value, and upscaler version. Settings also has toggles for the `/stealth` and `/public` commands.
4. You can use the **`/show`** command with the unique Job ID to move a job to another server or channel, revive a lost job, or refresh an old job to make new variations, upscale, or use newer parameters and features.
    - /show only works on your own jobs.
5. The **`/blend`** command allows you to upload 2–5 images quickly and then looks at the concepts and aesthetics of each image and merges them into a novel new image.
    - /blend is the same as using multiple image prompts with /imagine, but the interface is optimized for easy use on mobile devices.
    - /blend works with up to 5 images. To use more than 5 images in a prompt use image prompts with /imagine
    - /blend does not work with text prompts. To use text and image prompts together, use image prompts and text with /imagine
6. The **`/describe`** command allows you to upload an image and generate four possible prompts based on that image. Use the /describe command to explore new vocabulary and aesthetic movements.
    - /describe generates prompts that are inspirational and suggestive, it cannot be used to recreate an uploaded image exactly.
    - /describe returns the aspect ratio for uploaded images.
7. Activate Remix mode with the **`/prefer remix`** command to change prompts, parameters, model versions, or aspect ratios between variations.
8. Use the **`/ask`** command to get answers to many common **support** questions.
9. **`/shorten`** lets you 'analyze' a prompt and get suggestions on what words might not be doing anything and which ones might be key. **this is an experimental feature and might not give the expected results.**

# **Create a Prompt**

Start with the **`/imagine`** command followed by your text prompt. For example, **`/imagine a serene beach at sunset`**.

## Use **Image Prompts**

You can use images as part of a prompt to influence a Job's composition, style, and colors. Images prompts can be used alone or with text prompts—experiment with combining images with different styles for the most exciting results.

To add images to a prompt, type or paste the web address where the image is stored online. **The address must end in an extension like .png, .gif, or .jpg**. After adding image addresses, add any additional text and parameters to complete the prompt.

![Image showing the Midjourney prompt structure](How%20to%20Midjourney/MJ_Prompt.png)

Image showing the Midjourney prompt structure

If the **image is online:**

1. In most browsers, right-click or long-press an image and select Copy Image Address to get the URL.
2. Drag the image file into the prompt box to add the image's URL, or right-click and paste the link within the prompt box.

If the **image is on your computer or phone**, you can send it as a message to the Midjourney Bot first to generate a link:

1. Paste the image into the chat with Midjourney Bot. Press Enter to send your image.
2. **PC**: Right-click on the image and select "Copy Link" (NOT "Copy Message Link").
**Mobile**: Tap and hold on the image, then select "Copy Media Link.”
3.  paste the link within the prompt box.

<aside>
☝ Upload images in your Direct Messages with the Midjourney Bot to prevent other server users from seeing an image.

</aside>

- Image prompts go at the **front** of a prompt.
- Prompts must have **two images or one image and text to work.**
- An image URL must be a **direct** link to an online image.
- Your file should end in **.png, .gif, .webp, .jpg, or .jpeg.**
- The `/blend` command is a simplified image prompting process optimized for mobile users.
- Image prompts are **visible** on the Midjourney website unless a user has **Stealth Mode**.

### Image Weights (--iw)
In --v 5 you can increase the influence of your reference image using --iw N where N is a value between 0 and 2. 
The default is 1.0 so if you want your image reference to be less influential, try --iw 0.5  and if you want it to be very influential try --iw 2.  (The iw stands for image weight.)

Reference image recommendations:
- Play  with --iw N. All images will have the weight value of N. You can't give images different values.
- Play with the value of --stylize (--s) between 0 and 1000 to turn down (or up) the influence of Midjourney's house style.
- The URL of your reference image(s) MUST end in an image filename extension such as png, jpg, gif.
- Strive to use the same aspect ratios for input  and output: 1:1 in for 1:1 out. 2:3 in for 2:3 out, etc.
- Reference images should be simple. Clear subjects, uncomplicated backgrounds.
- You can't use URLs in place of words in the prompt. Click here for more information: https://discord.com/channels/662267976984297473/1026944423692619878/1058176989900582912
- Image refs work best if they already represent roughly what you want to see in the final image.
- MJ will always create a brand new image, never a copy. You can't recreate the source image. You'll only get rough likenesses of the people in the pictures.
- Midjourney will NOT invent/add/create by itself. You must prompt for it. A reference image that does not include arms will continue to not have arms, unless your prompt mentions arms, i.e. sleeves, biceps, or bracelets.
- You can add/remove image references using remix. This creates some cool opportunities. Try it out.

## **Use parameters**

Customize your image generation using various parameters. 

[Midjourney Parameter List](https://docs.midjourney.com/docs/parameter-list)

### **Default Values (Model Version 5, 5.1, and 5.2)**

|  | Aspect Ratio | Chaos | Quality | Seed | Stop | Stylize |
| --- | --- | --- | --- | --- | --- | --- |
| Default Value | 1:1 | 0 | 1 | Random | 100 | 100 |
| Range | any | 0–100 | .25 .5, or 1 | whole numbers 0–4294967295 | 10–100 | 0–1000 |
1. **`--version` or `--v`**: This parameter allows you to choose a model version. Each model excels at producing different types of images. 
    - **Midjourney** supports different model versions, each excelling at producing different types of images. Use the `**-version`** or `**-v`** parameter to choose a model. For example, `**-v 5.2`** for the latest model.
        
        interesting article that compares the versions here: 
        
        [All Midjourney Versions Compared [V1-V5 Evolution] - AiTuts](https://aituts.com/midjourney-versions/)
        
    - The **Niji** model is a collaboration between Midjourney and [Spellbrush](https://spellbrush.com/) tuned to produce anime and illustrative styles with vastly more knowledge of anime, anime styles, and anime aesthetics. It's excellent at dynamic and action shots and character-focused compositions.
        
        To use this model, add the **`--niji 5`** parameter to the end of a prompt, or use the **`/settings`** command and select **`🍏 Niji version 5`**
        
2. The **`--aspect`** or **`--ar`** parameter changes the aspect ratio of the generated image. An aspect ratio is the width-to-height ratio of an image. It is typically expressed as two numbers separated by a colon, such as 7:4 or 4:3.
    
    [What Are Common Aspect Ratios for Images?](https://marketing.istockphoto.com/blog/aspect-ratio/)
    
    - Aspect ratios greater than 2:1 are experimental and may produce unpredictable results.
    - The default aspect ratio is 1:1.
    - --aspect must use **whole numbers**. Use 139:100 instead of 1.39:1.
    - The aspect ratio impacts the shape and composition of a generated image.
    - Some aspect ratios may be slightly changed when upscaling.
3. **`--stylize`**: This parameter influences the artistic style of the generated image. A higher value means all the options will look more “refined” (i.e. artistic color, composition, and forms).
    
    comparison of **stylize** parameter for the prompt **`a woman with a mental illness, illustration -v 5.2 --chaos 25`:**
    
    ||||||
    | --- | --- | -- | -- | -- |
    | ![stylize = 15](How%20to%20Midjourney/grumpykitten9741_a_woman_with_a_mental_illness_illustration_4da0d3b5-c800-4a1d-83a8-5fe2d96f2a3c_c25_s15.png)  `stylize = 15` |  ![stylize = 100](How%20to%20Midjourney/grumpykitten9741_a_woman_with_a_mental_illness_illustration_4f17e4ca-2c5f-49df-a554-6fb5c054ba8d_c25_s100.png) `stylize = 100` | ![stylize = 200](How%20to%20Midjourney/grumpykitten9741_a_woman_with_a_mental_illness_illustration_095ed995-7804-44e2-963f-dff9d065850d_c25_s200.png) `stylize = 200` | ![stylize = 500](How%20to%20Midjourney/grumpykitten9741_a_woman_with_a_mental_illness_illustration_87dd2b2c-e2bb-493d-a981-d830de7dcfba_c25_s500.png) `stylize = 500` | ![stylize = 1000](How%20to%20Midjourney/grumpykitten9741_a_woman_with_a_mental_illness_illustration_4fb315f1-e75a-413a-bb33-d87f67d35bdc_c25_s1000.png)  `stylize = 1000` | 
    
    - If you used `--stylize` in V4/V5.0/V5.1 you may need to re-adjust your numbers for V**5.2**, Try reducing it by much as **5x**. Meaning `--stylize 1000` V5/V5.1 should be a `--stylize 200` prompt for V5.2
4. **`--chaos`**: This parameter introduces randomness into the image generation process. It accepts values from 0 to 1000, with 0 being no chaos and 1000 being maximum chaos. For example, **`/imagine a serene beach at sunset --chaos 500`** will generate an image of a beach at sunset with moderate randomness. **a higher chaos value means high variance; with a low value, the results will be closer to the most popular depictions of the prompt.**
    
    comparison of **chaos** parameter for the prompt **`a woman with a mental illness, illustration --v 5.2 --stylize 200`**:
    
    
    ||||||
    | --- | --- | -- | -- | -- |
    | ![chaos = 10](How%20to%20Midjourney/grumpykitten9741_a_woman_with_a_mental_illness_illustration_248042d5-ea26-4bde-a1ec-186d00ff1f75_c10_s200.png)   `chaos = 10` |   ![chaos = 25](How%20to%20Midjourney/grumpykitten9741_a_woman_with_a_mental_illness_illustration_1c03b0d7-563b-46a8-a365-ff16dc63649e_c25_s200.png) `chaos = 25` | ![chaos = 50](How%20to%20Midjourney/grumpykitten9741_a_woman_with_a_mental_illness_illustration_a9705dab-bbbb-4159-aa33-e4b95ec224bd_c50_s200.png) `chaos = 50` |   ![chaos = 75](How%20to%20Midjourney/grumpykitten9741_a_woman_with_a_mental_illness_illustration_f9cf0046-63fd-48ea-a9cd-ddee4a0358fb_c75_s200.png) `chaos = 75` | ![chaos = 100](How%20to%20Midjourney/grumpykitten9741_a_woman_with_a_mental_illness_illustration_fdc4bb28-0b9a-44e4-97de-3e548356d918_c100_s200.png) `chaos = 100` |
    
5. **`--tile`**: This parameter generates images that can be used as repeating tiles to create seamless patterns. For example, **`/imagine a pattern of leaves --tile`** will generate a tile of a leaf pattern that can be repeated seamlessly.
6. **`--repeat`**: This parameter runs a job multiple times. It accepts values from 2 to 10/40 (Standard/Pro subscriptions only). For example, **`/imagine a serene beach at sunset --repeat 5`** will generate 5 different images of a serene beach at sunset.
7. **`--quality`**: controls the quality of the generated image. For example, **`/imagine a serene beach at sunset --quality 0.25`**  will generate a low-quality image of a beach at sunset. 
8. **`--seed`**: This parameter allows you to specify a seed for the image generation process. This can be useful if you want to generate the same image again in the future. For example, **`/imagine a serene beach at sunset --seed 12345`** will generate an image based on the seed value of 12345. 
    
    <aside>
    ☝ To get the seed number for a past image, [copy the job ID](https://docs.midjourney.com/docs/show-job) and use the **`/show <Job ID #>`** command with that ID to revive the Job.
    
    </aside>
    
9. Use the **`--stop`** parameter to finish a Job partway through the process. Stopping a Job at an earlier percentage can create blurrier, less detailed results.
    - --stop accepts values: 10–100.
    - The default --stop value is 100.
    - --stop does not work while Upscaling.

    |||||
    | --- | --- |--|--|
    | ![`stop = 10`](How%20to%20Midjourney/grumpykitten9741_a_serene_beach_at_sunset_41f89c7c-a8a6-4c5c-a90a-387a1d00ffac.png) `stop = 10`|   ![`stop = 50`](How%20to%20Midjourney/grumpykitten9741_a_serene_beach_at_sunset_35f225b5-71d4-4a8e-904e-5c95eadc56b2.png)`stop = 50` |  ![`stop = 75`](How%20to%20Midjourney/grumpykitten9741_a_serene_beach_at_sunset_2111c897-a7dc-40f0-a0a5-c6ce22ce677b.png)`stop = 75` |   ![`stop = 100`](How%20to%20Midjourney/grumpykitten9741_a_serene_beach_at_sunset_4005d30c-29ed-4218-9a9d-0bfb51efeb6d.png)`stop = 100`
    
10. ****`--style`****: fine-tunes the aesthetic of some [Midjourney Model Versions](https://docs.midjourney.com/models). Adding a style parameter can help you create more photo-realistic images, cinematic scenes, or cuter characters. 
    
    Default Model Version **5.2** and the previous version **5.1** accept
    
    - `--style **raw`** (reduces Midjourney default aesthetic)
    
    Model Version **Niji 5** accepts
    
    - `--style cute`
    - `--style scenic`
    - `--style original`
    - `--style expressive`
    
    Comparison of styles for the prompt “**a serene beach in sunset”:**
    ||||||
    | --- | --- | --- |--|--|
    |    ![**--v 5.2 --style raw**](How%20to%20Midjourney/grumpykitten9741_a_serene_beach_in_sunset_136965b1-17cd-431b-ac52-bbce6b821c2b_v52_raw.png) **--v 5.2 --style raw** | ![**--niji 5 --style original**](How%20to%20Midjourney/grumpykitten9741_a_serene_beach_in_sunset_7ed8db69-827e-45c5-a834-b76904902419_niji5_original.png) **--niji 5 --style original**  |  ![**--niji 5 --style scenic**](How%20to%20Midjourney/grumpykitten9741_a_serene_beach_in_sunset_ce0007c9-d1c8-45db-8d9e-2ede99ac968a_niji5_scenic.png) **--niji 5 --style scenic**    |    ![**--niji 5 --style expressive**](How%20to%20Midjourney/grumpykitten9741_a_serene_beach_in_sunset_be861ec1-80c8-4b6c-9053-567236347c43_niji5_expressive.png)   **--niji 5 --style expressive**   |  ![**--niji 5 --style cute**](How%20to%20Midjourney/grumpykitten9741_a_serene_beach_in_sunset_b71c19cc-fbe3-427a-b0d3-ba9028a571f3_niji5_cute.png) **--niji 5 --style cute**   |
11. **Experimental `--weird` command**
    - This command makes your images look more weird/edgy
    - Do not consider this a stable feature, what's weird may change over time
    - It goes from `-weird 0` to `-weird 3000`
    - The strength of this command is dynamic with the prompt (you may need to adjust it prompt-to-prompt)
    - We recommend starting with smaller values such as 250 or 500.
    - If you want it to look weird AND pretty you should try using `-stylize` along with your weird
    - If you use `-stylize` with weird we recommend using a equal value for both parameters
    - Combining `-weird` with `-seed` is a bit messed up right now, make sure you set `-weird 0` if you want to do comparisons

## **Use Multi-Prompts**

You can have the bot consider two or more separate concepts **individually** using `**::`** as a separator. For example, `**hot:: dog`** will consider "hot" and "dog" as separate concepts. 

- **for v5+:** Use weights for multi-prompts (for instance, **`**space::2 ship`). Remember: Weights are normalized. values are in the range .5–2.**
- Negative weights can be added to prompts to remove unwanted elements. **The sum of all weights must be a positive number.**
- The **`--no`** [parameter](https://docs.midjourney.com/no): is the same as weighing part of a multi prompt to "-.5" `**vibrant tulip fields:: red::-.5`** is the same as `**vibrant tulip fields --no red`**.

## Use **Permutation Prompts**

allow you to quickly generate variations of a Prompt with a single /imagine command. By including lists of options separated with commas, within curly braces {} in your prompt, you can create multiple versions of a prompt with different combinations of those options.

You can use Permutation Prompts to create combinations and permutations involving any part of a Midjourney Prompt, including text, image prompts, parameters, or prompt weights.

**Prompt Example:**

**`/imagine prompt`** **`a {red, green, yellow} bird`** creates and processes three Jobs:

`/imagine prompt` `a red bird`

`/imagine prompt` `a green bird`

`/imagine prompt` `a yellow bird`

- Permutation prompts are only available while using **Fast mode**.
- **Basic** Subscribers can create a maximum of **4** Jobs with a single Permutation Prompt.
- **Standard** Subscribers can create a maximum of **10** Jobs with a single Permutation Prompt.
- **Pro** Subscribers can create a maximum of **40** Jobs with a single Permutation Prompt.
- The Midjourney Bot processes each Permutation Prompt variation as an **individual Job**. Each Job consumes GPU minutes.
- Permutation Prompts will show a **confirmation message** before they begin processing.

# Upscalers

![Screenshot_33.png](How%20to%20Midjourney/Screenshot_33.png)

**The newest [Midjourney Model Version 5](https://docs.midjourney.com/models) (and Niji 5) produces high-resolution 1024 x1024 px image grids without needing an additional step to upscale each image. When using the latest Midjourney Models the `U1` `U2` `U3` `U4` buttons under each image grid will separate the selected image from the initial image grid for easy saving and downloading.**

## **Midjourney Dimensions and Sizes**

*All sizes are for square 1:1 aspect ratios.*

| Model Version | Starting Grid Images Size | Model Version 4 Default Upscaler |
| --- | --- | --- |
| Version 5 | 1024 x 1024 | - |
| Version 4 | 512 x 512 | 1024 x 1024 |
| niji 5 | 1024 x 1024 | - |
| niji 4 | 512 x 512 | 1024 x 1024 |

<aside>
☝ Earlier Midjourney versions start by generating a grid of **low-resolution** image options for each Job. You can use a Midjourney upscaler on any of these images to **increase the size and add additional details**. **Using an upscaler uses your subscription's GPU minutes.**

</aside>

|||
|--|--|
| ![**a serene beach in sunset --v 1**](How%20to%20Midjourney/grumpykitten9741_a_serene_beach_in_sunset_ed0a2c0d-9915-4cac-ba69-73c04730e964_v1.png)**a serene beach in sunset --v 1** | ![Upscaled option 1](How%20to%20Midjourney/grumpykitten9741_a_serene_beach_in_sunset_5dbb8e19-a8f1-4838-a290-771563a5fc16_v1_up.png) Upscaled option 1 |

## **Remaster**

Remaster is an option for upscaled images made with previous [Midjourney Model Versions](https://docs.midjourney.com/legacy/docs/upscalers). Remaster will create a new grid of images blending the composition of the original image.

# Zoom Out

![Screenshot_34.png](How%20to%20Midjourney/Screenshot_34.png)

The Zoom Out option allows you to extend the canvas of an upscaled image beyond its original boundaries without changing the content of the original image. The newly expanded canvas will be filled-in using guidance from the prompt and the original image.

<aside>
☝ `**Zoom Out`** does not increase the maximum 1024px x 1024 px size of an image.

</aside>

|||
|--|--|
| ![Original, ar 1:1](How%20to%20Midjourney/grumpykitten9741_a_simple_floral_arrangement_in_spring_colors_o_7b70e8ef-69b9-4136-b1b9-97cfedb3e3a6.png) Original, ar 1:1 | ![zoom out x2 ar 9:16](How%20to%20Midjourney/grumpykitten9741_a_simple_floral_arrangement_in_spring_colors_o_23b9c0ea-6465-4c73-945a-8a597d404d5a.png) zoom out x2 ar 9:16 |

## **Custom Zoom**

The `**🔎 Custom Zoom`** button lets you choose how much to zoom out on an image. `**🔎 Custom Zoom`** button under an upscaled image will pop up a dialogue box where you enter a custom value for **`--zoom`**. **`--zoom`** accepts values between 1-2.

![Screenshot_37.png](How%20to%20Midjourney/Screenshot_37.png)

`**🔎 Custom Zoom` allows you to [change the prompt](https://docs.midjourney.com/remix) before you expand your image**, giving you finer control over the finished image.

<aside>
☝ **Change the Aspect Ratio of an Upscaled Image:** You can use **`--zoom 1`** in this `**Custom Zoom`** pop-up box to change the **[aspect ratio](https://docs.midjourney.com/aspect-ratios)**, with the **`--ar`** parameter without zooming out.

</aside>

|||
|--|--|
| ![**a simple floral arrangement in spring colors, one main element, leaves, gouache, illustration, minimalistic, clean lines --no vase --niji 5 --style expressive --ar 9:16,** after custom zoom out and change of aspect ratio](How%20to%20Midjourney/grumpykitten9741_a_simple_floral_arrangement_in_spring_colors_o_9a252777-958c-46dd-920c-6efdefe38c67.png) **a simple floral arrangement in spring colors, one main element, leaves, gouache, illustration, minimalistic, clean lines --no vase --niji 5 --style expressive --ar 9:16,** after custom zoom out and change of aspect ratio | ![new prompt: **A framed picture on the wall --ar 3:2 --zoom 2**](How%20to%20Midjourney/grumpykitten9741_A_framed_picture_on_the_wall_b61a3e7c-ddf3-4a35-a0b9-813a056034b1.png) new prompt: **A framed picture on the wall --ar 3:2 --zoom 2** |

# Pan

![Screenshot_38.png](How%20to%20Midjourney/Screenshot_38.png)

- Underneath your upscales you'll see arrow buttons, If you click an arrow it will extend your image in that direction
- If you type `/settings` and click `Remix mode` you'll have the option to change your prompt as you extend your image. Use this to tell panoramic stories!
- As you pan out your image we will keep extending it even though the resolution will become very large
- Yes, that means you can keep panning multiple times!
- **Variations** are **not supported** on panned images
- If you **zoom out** on a panned image its resolution will decrease back down to **default size**
- You **cannot pan both horizontally and vertically** on the same image
- You **cannot control** the amount you pan with each panning operation
- You may see 'repetition' as you pan, to avoid this try changing your prompt as you go to include new details

||||
|--|--|--|
| ![**a serene beach in sunset --v 5.2**](How%20to%20Midjourney/grumpykitten9741_a_serene_beach_in_sunset_416ead0a-ed60-474b-acdf-21cff3085580.png) **a serene beach in sunset --v 5.2** | ![panned left](How%20to%20Midjourney/grumpykitten9741_a_serene_beach_in_sunset_bc1d43df-a981-41d2-acd0-665542c941e8.png) panned left | ![panned left x2](How%20to%20Midjourney/grumpykitten9741_a_serene_beach_in_sunset_bd06f8e5-9115-4672-a4d7-baf72ada9427.png) panned left x2 |

# **Variation Mode**

- **"High Variation Mode" is** turned on by default and makes all variation jobs much more varied.
- To toggle this type /settings and click a different variation mode.
- Underneath all upscales you can also chose which strength of variation you want.

![Untitled](How%20to%20Midjourney/Untitled.png)

# Earn Free Hours

Subscribers can earn a free Fast GPU hour each day by rating images. A bonus Fast hour is awarded to the top 2000 raters each day.

- Bonus hours expire 30 days from the date they are awarded.
- You must have an active subscription to participate.
- You can see how many hours you have earned rating images on your [Midjourney.com/account](https://www.midjourney.com/account/) page in the **Bonus** category.

## **How to Rate Images**

Current subscribers can rank image pairs at [midjourney.com/app/rank-pairs/](https://www.midjourney.com/app/rank-pairs/) to earn free Fast GPU hours. Click on the image you like the most for each pair that is presented. 

Rankings are based on personal preference, so choose the image **you like the most** based on appearance, effort, colors, concept, or theme.

# Extras

[Unique Ideas to Make Money with AI Art - AiTuts](https://aituts.com/make-money-with-ai-art/)

[Midjourney vs. human illustrators: has AI already won?—Martian Chronicles, Evil Martians’ team blog](https://evilmartians.com/chronicles/midjourney-vs-human-illustrators-has-ai-already-won)