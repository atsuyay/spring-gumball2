# CMPE 172 - Lab #10 - DevOps CI/CD Notes

## CI Workflow (Spring Gumball) 

![CI Java CI with Gradle](images/CI_build.PNG) Figure 1. Shows successful workflow of Java CI with Gradle

## CD Workflow (Spring Gumball) 


### Challenges Encountered
I had challenges with gke-credentials and have to give permission when creating the GKE Service Account as my CD builds were failing before giving permissions.

![1Find your GKE Project ID1](https://github.com/atsuyay/spring-gumball2/assets/60360870/3debcd61-e80a-4baf-a586-820d33f9e37c)
![2gcloud config get project](https://github.com/atsuyay/spring-gumball2/assets/60360870/e1d78922-840b-42b7-b3c6-d53e4334c3fe)
![3activationAPI](https://github.com/atsuyay/spring-gumball2/assets/60360870/aa8d4509-e2f2-43be-add3-b2bd7652b46a)
![4Create Service Account](https://github.com/atsuyay/spring-gumball2/assets/60360870/861e8903-3a2f-46e8-a953-ea9482f88f49)
![5Create Service Account2](https://github.com/atsuyay/spring-gumball2/assets/60360870/923b01e1-746e-44fa-92ae-c120e0f997c4)
![6IMF roles](https://github.com/atsuyay/spring-gumball2/assets/60360870/7c640422-01d0-4cbe-8fb9-c9d70ecd4b12)
![7 grant access1](https://github.com/atsuyay/spring-gumball2/assets/60360870/91f691d9-e19a-41bd-bd47-a4d98d549872)
![8 before making new key](https://github.com/atsuyay/spring-gumball2/assets/60360870/959d6211-23d6-4480-882d-d469dfbb9018)
![9 permission complete](https://github.com/atsuyay/spring-gumball2/assets/60360870/80a66c3f-0db4-4590-892f-53db1e5b4dd3)
![11 new key generated](https://github.com/atsuyay/spring-gumball2/assets/60360870/ecd643c9-e5d8-4be3-9a07-bb388d05dad3)
![12 befor make github key](https://github.com/atsuyay/spring-gumball2/assets/60360870/bc0a283d-0b67-4afa-b24a-667cf99eca72)
![12 create new key done](https://github.com/atsuyay/spring-gumball2/assets/60360870/fab49835-a4db-448e-972f-e16ae0dd1431)
![13 New Repository Secret GKE_PROJECT](https://github.com/atsuyay/spring-gumball2/assets/60360870/a8d180f2-0880-4470-9d0a-251d795b22a3)
![14 gke sa key](https://github.com/atsuyay/spring-gumball2/assets/60360870/3306cf60-0c61-44e0-bd9a-959b0ec2c593)
![15 two key made](https://github.com/atsuyay/spring-gumball2/assets/60360870/29191b42-511f-40f6-a4cb-20532cffc0d2)
![16 Trigger a CD Deployment by creating a new GitHub Releas](https://github.com/atsuyay/spring-gumball2/assets/60360870/a5ddf582-e503-4e05-b287-539d0752bc00)
![17 github new release](https://github.com/atsuyay/spring-gumball2/assets/60360870/9f87b7bb-838d-4259-9dbb-a9e59e708722)
![18 new release done](https://github.com/atsuyay/spring-gumball2/assets/60360870/3dd5cd67-9cec-43c5-88c7-ce9d6963c777)
![19 github build done](https://github.com/atsuyay/spring-gumball2/assets/60360870/6bd79c20-31bc-4882-ac35-45c32fb3bbbd)
![19 service on gke](https://github.com/atsuyay/spring-gumball2/assets/60360870/7ba7fb50-50ac-4436-9516-04ad16ecc9c5)
![20 gke work load](https://github.com/atsuyay/spring-gumball2/assets/60360870/d5923f90-9402-4422-9937-9b852dab19a9)
![20 overall of github](https://github.com/atsuyay/spring-gumball2/assets/60360870/7c706f6f-75b5-4677-af49-5b002f0b22e4)
![21 gke service2](https://github.com/atsuyay/spring-gumball2/assets/60360870/94bd516a-e195-4a65-a97a-b54ec72d3c8a)
![22 gke network](https://github.com/atsuyay/spring-gumball2/assets/60360870/93baec37-dd20-418f-9409-89187fe23d3a)
![23 gke ingress load balancer](https://github.com/atsuyay/spring-gumball2/assets/60360870/a0bf0063-6cfa-4465-bc04-924cb7c5a0d1)
![24 load balance created](https://github.com/atsuyay/spring-gumball2/assets/60360870/ddaf7743-4de2-4871-9a43-694fb7bf4d17)
![25 gumball machine](https://github.com/atsuyay/spring-gumball2/assets/60360870/3b40f544-c3f3-4fb4-916a-4c767ad684e4)
