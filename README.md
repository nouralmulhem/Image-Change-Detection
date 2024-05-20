# Image Change Detection

<img src="https://i.giphy.com/Ym5Urkj7ReOdCcxLud.webp"/>

    This repository contains the code and documentation for a Change detection project, the model achived a Jaccard Index score of 61% on unseen data, this model secured the 5th place in the competition of Cairo University Faulty of Engineering

The project uses two approaches:

- Traditional Approach
- Deep Learning Approach 


## <img align= center width=50px height=50px src="https://user-images.githubusercontent.com/71986226/154075883-2a5679d2-b411-448f-b423-9565babf35aa.gif"> Table of Contents
- <a href ="#Overview">Overview</a>
- <a href ="#started"> Get Started</a>
- <a href ="#modules"> Modules</a>
- <a href ="#contributors">Contributors</a>
- <a href ="#license">License</a>

## <img align="center"  height =50px src="https://user-images.githubusercontent.com/71986226/154076110-1233d7a8-92c2-4d79-82c1-30e278aa518a.gif"> Project Overview <a id = "Overview"></a>

The objective was to make a change detection model to detect changes in satellite imagery.

For example:

- No change
![nochange](images/image.png)
- Change
![change](images/image-2.png)

## <img  align= center width=50px height=50px src="https://c.tenor.com/HgX89Yku5V4AAAAi/to-the-moon.gif"> Get Started <a id = "started"></a>

To get started with the project, follow these steps:

1. Clone the repository.
2. Dont froget to trun on GPU of you are using Colab or Kaggle notebook.
3. Customize the code and add any additional features as needed.
4. Run the last cell of interface and enjoy

## <img  align= center width=50px height=50px src="https://cdn.pixabay.com/animation/2022/07/31/06/27/06-27-17-124_512.gif"> Modules <a id ="modules"></a>

### First the Deep Learning Approach

Our approach used basically Unet plus plus model along with se_resnet101 as an encoder.

- Our approach utilized the Unet++ model architecture coupled with se_resnet101 as an encoder.
- The Unet++ architecture, known for its ability to capture complex features effectively, was chosen over the standard Unet model due to its superior performance in capturing intricate features.
- Additionally, the use of se_resnet101 as our encoder was based on recommendations from prior literature surveys.
- This selection was made to leverage the proven effectiveness of se_resnet101 in feature extraction tasks, aligning with the goals of our study.

![alt text](images/image-3.png)

![alt text](images/image-4.png)

Our data set was of

- image 1: image before change
- image 2: image after change
- mask: the change in the image

### Second the Traditional Approach

We used 2 different traditional approaches to achieve our goal of change detection.

- We used otsu's thresholding algorithm to obtain the threshold value based on intensity distribution among the pixels in the image.

The thresholding algorithm tries to get an equal number of pixels above and below its intensity.

- Image differencing + otsu as a thresholding algorithm

- CVA + otsu as a thresholding algorithm

## <img  align= center width=50px height=50px src="https://cdn.pixabay.com/animation/2022/07/31/06/27/06-27-17-124_512.gif"> Results <a id ="results"></a>

<table >
<thead>
    <tr>
      <th style="text-align:center;">A</th>
      <th style="text-align:center;">B</th>
      <th style="text-align:center;">Prediction</th>
      <th style="text-align:center;">Ground Truth</th>
    </tr>
  </thead>
  <tr>
        <td align="center"><img src="./results/A/0074.png" width="150px;" alt="A"/><br /></td>
        <td align="center"><img src="./results/B/0074.png" width="150px;" alt="A"/><br /></td>
        <td align="center"><img src="./results/ground truth/0074.png" width="150px;" alt="A"/><br /></td>
        <td align="center"><img src="./results/predictions/0074.png" width="150px;" alt="A"/><br /></td>
  </tr>
  <tr>
        <td align="center"><img src="./results/A/0104.png" width="150px;" alt="A"/><br /></td>
        <td align="center"><img src="./results/B/0104.png" width="150px;" alt="A"/><br /></td>
        <td align="center"><img src="./results/ground truth/0104.png" width="150px;" alt="A"/><br /></td>
        <td align="center"><img src="./results/predictions/0104.png" width="150px;" alt="A"/><br /></td>
  </tr>
  <tr>
        <td align="center"><img src="./results/A/0572.png" width="150px;" alt="A"/><br /></td>
        <td align="center"><img src="./results/B/0572.png" width="150px;" alt="A"/><br /></td>
        <td align="center"><img src="./results/ground truth/0572.png" width="150px;" alt="A"/><br /></td>
        <td align="center"><img src="./results/predictions/0572.png" width="150px;" alt="A"/><br /></td>
  </tr>
</table>


<hr style="background-color: #4b4c60"></hr>
<a id ="Contributors"></a>

## <img align="center"  height =60px src="https://user-images.githubusercontent.com/63050133/156777293-72a6e681-2582-4a9d-ad92-09d1181d47c7.gif"> Contributors <a id ="contributors"></a>

<br>
<table >
  <tr>
        <td align="center"><a href="https://github.com/Ahmed-H300"><img src="https://avatars.githubusercontent.com/u/67925988?v=4" width="150px;" alt=""/><br /><sub><b>Ahmed Hany</b></sub></a><br /></td>
        <td align="center"><a href="https://github.com/nouralmulhem"><img src=https://avatars.githubusercontent.com/u/76218033?v=4" width="150px;" alt=""/><br /><sub><b>Nour Ziad</b></sub></a><br /></td>
        <td align="center"><a href="https://github.com/EslamAsHhraf"><img src=https://avatars.githubusercontent.com/u/71986226?v=4" width="150px;" alt=""/><br /><sub><b>Eslam Ashraf</b></sub></a><br /></td>
        <td align="center"><a href="https://github.com/ahmedmadbouly186"><img src=https://avatars.githubusercontent.com/u/66012617?v=4" width="150px;" alt=""/><br /><sub><b>Ahmed Madbouly</b></sub></a><br /></td>

  </tr>
</table>

<hr style="background-color: #4b4c60"></hr>

<a id ="License"></a>

## 🔒 License <a id ="license"></a>

> **Note**: This software is licensed under MIT License, See [License](https://github.com/nouralmulhem/Image-Change-Detection/blob/main/LICENSE).

