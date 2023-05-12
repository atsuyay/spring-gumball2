# CMPE 172 - Lab #10 - DevOps CI/CD Notes

## CI Workflow (Spring Gumball) 
![41 building](https://github.com/atsuyay/spring-gumball2/assets/60360870/bbb0b761-1ace-4a74-b59c-573c6e361f9f)
![42 build done](https://github.com/atsuyay/spring-gumball2/assets/60360870/6b9aeeff-1607-4558-a161-571e140fbe2b)



## CD Workflow (Spring Gumball) 


### Challenges Encountered
I had challenges with gke-credentials and have to give permission when creating the GKE Service Account as my CD builds were failing before giving permissions.

![1Find your GKE Project ID1](https://github.com/atsuyay/spring-gumball2/assets/60360870/2dd8da6a-7b52-4e85-8e93-65059af401b2)
I created a GKE named CMPE172.
プロジェクト名--> Project Name
![1Find your GKE Project ID1](https://github.com/atsuyay/spring-gumball2/assets/60360870/2dd8da6a-7b52-4e85-8e93-65059af401b2)
run "gcloud config get project"
![2gcloud config get project](https://github.com/atsuyay/spring-gumball2/assets/60360870/880fc205-4e71-4c2e-b40b-d2e37dca37ab)
Enabling access to APIs
![3activationAPI](https://github.com/atsuyay/spring-gumball2/assets/60360870/cba402e3-3ca6-46b8-be9a-b0510f808c03)
Setting account details
![4Create Service Account](https://github.com/atsuyay/spring-gumball2/assets/60360870/6bf79040-c858-47cd-b3da-088eb464c24a)
Service Account created
![5Create Service Account2](https://github.com/atsuyay/spring-gumball2/assets/60360870/50a921b6-50c6-4f43-9ecb-21b915616332)

Setting of Permissions for this project.
![6IMF roles](https://github.com/atsuyay/spring-gumball2/assets/60360870/4f64b17f-7878-4076-bfd3-defb31b76862)

Before making key
![8 before making new key](https://github.com/atsuyay/spring-gumball2/assets/60360870/9dae95ca-246d-4e10-9790-320105d2ed60)

key setting
![9 permission complete](https://github.com/atsuyay/spring-gumball2/assets/60360870/641c162e-30f0-447e-aee8-fd68c4dbfe7e)

Key created.
![11 new key generated](https://github.com/atsuyay/spring-gumball2/assets/60360870/a880da2e-ffd1-4039-a8f5-90a2c38a83f2)

key created.
![12 create new key done](https://github.com/atsuyay/spring-gumball2/assets/60360870/ecd65189-e621-4d91-9bc0-f71985975fe2)

Docker setting begin
![12 befor make github key](https://github.com/atsuyay/spring-gumball2/assets/60360870/5ab0c521-a79a-4b2d-baf7-6aa7205c74b5)

New Secret key created (GKE_PROJECT)
![13 New Repository Secret GKE_PROJECT](https://github.com/atsuyay/spring-gumball2/assets/60360870/c8efba82-5d70-4bd4-b0b6-8a4f1b16dc75)

New Secret key created (GKE_SA_KEY)
![14 gke sa key](https://github.com/atsuyay/spring-gumball2/assets/60360870/7c45e44b-f699-4818-bdfd-24561f170d0c)

Two keys made
![15 two key made](https://github.com/atsuyay/spring-gumball2/assets/60360870/87298c1a-7e8d-4f9c-abb8-80c608b26066)

Trigger a CD Deployment by creatting a new Github Release
![16 Trigger a CD Deployment by creating a new GitHub Releas](https://github.com/atsuyay/spring-gumball2/assets/60360870/c2110a92-e19c-44e2-a667-57c36a4b932f)

Make new release 
![17 github new release](https://github.com/atsuyay/spring-gumball2/assets/60360870/b4031dd7-7ccd-4a38-a819-b27664b20354)

New Release created
![18 new release done](https://github.com/atsuyay/spring-gumball2/assets/60360870/379de97b-b1c3-4443-b311-39514b8e4e5f)

Setup, Build, Publish, and Deploying
![19 github build done](https://github.com/atsuyay/spring-gumball2/assets/60360870/9e05e54f-effd-49f6-ae19-65614c6302f5)

Complete Setup, Build, Publish, and Deploy.
![20 overall of github](https://github.com/atsuyay/spring-gumball2/assets/60360870/7ef3d13e-dd07-4a80-8684-836922ee96d5)
![19 service on gke](https://github.com/atsuyay/spring-gumball2/assets/60360870/f9fcd8e4-49b5-4639-affb-013cde7fd0bd)
![20 gke work load](https://github.com/atsuyay/spring-gumball2/assets/60360870/91282891-7169-451b-8f97-699b52feab3a)
![21 gke service2](https://github.com/atsuyay/spring-gumball2/assets/60360870/6825e6bb-509c-42af-8ee2-dd0de6aa27d9)
![22 gke network](https://github.com/atsuyay/spring-gumball2/assets/60360870/80158473-ac80-401b-82e9-c3352b3bc0c3)
![23 gke ingress load balancer](https://github.com/atsuyay/spring-gumball2/assets/60360870/20df6aae-89f4-45ec-a431-4824c56c6fcb)
![24 load balance created](https://github.com/atsuyay/spring-gumball2/assets/60360870/85c29786-d6c1-4831-858f-da76003141e5)
![25 gumball machine](https://github.com/atsuyay/spring-gumball2/assets/60360870/e20cb7a6-a669-459a-a962-73fd016878ab)
