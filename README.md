# @rehat666/niji-api

A high-quality anime image generator API project by rehat666

## Preview

![Preview Image 1](./images/image_1.png)

![Preview Image 2](./images/image_2.png)

![Preview Image 3](./images/image_3.png)

![Preview Image 4](./images/image_4.png)


## Usage

```
npm install @rehat666/niji-api
```

```javascript
const { Niji } = require('@rehat666/niji-api');

const niji = new Niji("rehat"); // The main api key of the project do not change it!

(async () => {
  try {
    const generate = await niji.Create({
      prompt: '', // Prompt to generate text to image.
      imageUrl: '', // URL of the image for transforming an existing image with prompt.
      aspectRatio: '' // Ratio for adjusting the image aspect ratio in text to image not recommended for transforming existing images.
    });

    console.log(generate);
  } catch (error) {
    console.error(error);
  }
})();
```
## Thanks for using @rehat666/niji-api!
