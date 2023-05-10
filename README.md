# CMPE 172 - Lab #10 - DevOps CI/CD Notes

## CI Workflow (Spring Gumball) 

![CI Java CI with Gradle](images/CI_build.PNG) Figure 1. Shows successful workflow of Java CI with Gradle

## CD Workflow (Spring Gumball) 


### Challenges Encountered
I had challenges with gke-credentials and have to give permission when creating the GKE Service Account as my CD builds were failing before giving permissions.
![スクリーンショット 2023-05-09 15 51 53](https://github.com/atsuyay/spring-gumball2/assets/60360870/c5179f13-76c4-40ad-907d-de235e6543da)
![1Find your GKE Project ID1](https://github.com/atsuyay/spring-gumball2/assets/60360870/7f375577-2045-47cd-b5ac-559fe30d030d)
![スクリーンショット 2023-05-09 16 07 42](https://github.com/atsuyay/spring-gumball2/assets/60360870/e9385c89-b8bd-44c8-b7c5-9804b251a943)
![2Find your GKE Project ID](https://github.com/atsuyay/spring-gumball2/assets/60360870/69991674-0d07-4310-97bd-1498a6447f78)
![スクリーンショット 2023-05-09 16 12 40](https://github.com/atsuyay/spring-gumball2/assets/60360870/47398b66-c90a-48bf-837b-7fa05f3620c7)
![スクリーンショット 2023-05-09 16 12 47](https://github.com/atsuyay/spring-gumball2/assets/60360870/3c40308a-cb70-4284-9f95-a70188160d67)
![スクリーンショット 2023-05-09 16 13 16](https://github.com/atsuyay/spring-gumball2/assets/60360870/258d5d2b-9e39-4bcc-9a59-fd46fe37446b)
![スクリーンショット 2023-05-09 16 17 32](https://github.com/atsuyay/spring-gumball2/assets/60360870/66b387a8-8180-49d1-80f4-611dbd2117dd)
![スクリーンショット 2023-05-09 16 18 32](https://github.com/atsuyay/spring-gumball2/assets/60360870/627fee79-b845-489d-97d0-177afa872387)
![スクリーンショット 2023-05-09 16 20 00](https://github.com/atsuyay/spring-gumball2/assets/60360870/1b381075-3c81-4885-acc2-122c9342c3d6)
![スクリーンショット 2023-05-09 16 20 29](https://github.com/atsuyay/spring-gumball2/assets/60360870/321f53fa-7c47-4270-b2ef-c2e0299f2d3e)
![スクリーンショット 2023-05-09 16 21 01](https://github.com/atsuyay/spring-gumball2/assets/60360870/844ace00-be86-41cb-b290-386e107d9f41)
![スクリーンショット 2023-05-09 16 26 26](https://github.com/atsuyay/spring-gumball2/assets/60360870/4f669b5c-cac4-419e-880e-ff503f3cea01)
![スクリーンショット 2023-05-09 16 26 45](https://github.com/atsuyay/spring-gumball2/assets/60360870/d52188c5-04a6-429c-8647-ae121ddff60c)
![スクリーンショット 2023-05-09 16 28 04](https://github.com/atsuyay/spring-gumball2/assets/60360870/c1c3ec0f-cfd4-4233-8b16-5fa7ef59a6a3)
![スクリーンショット 2023-05-09 16 28 17](https://github.com/atsuyay/spring-gumball2/assets/60360870/b198aff0-c0ef-4be3-a5ce-b8efb32c165f)
![スクリーンショット 2023-05-09 16 28 43](https://github.com/atsuyay/spring-gumball2/assets/60360870/fa3d2c99-9d6f-4dbc-941e-0385c0de3920)
![スクリーンショット 2023-05-09 16 30 25](https://github.com/atsuyay/spring-gumball2/assets/60360870/461f4273-5978-463c-beb2-c5e2fdace3a1)
![スクリーンショット 2023-05-09 16 30 53](https://github.com/atsuyay/spring-gumball2/assets/60360870/4a43be8f-5ae6-4ae0-95eb-e2776be11fa3)
![スクリーンショット 2023-05-09 17 41 26](https://github.com/atsuyay/spring-gumball2/assets/60360870/8ef73925-5d6c-456e-8c41-6b06428dd3c3)
![スクリーンショット 2023-05-09 17 42 31](https://github.com/atsuyay/spring-gumball2/assets/60360870/bb96deee-653e-4691-9c55-bd67a8742681)
![スクリーンショット 2023-05-09 17 45 09](https://github.com/atsuyay/spring-gumball2/assets/60360870/cf53c8fe-c99f-4127-93f5-34fa1b25d013)
![スクリーンショット 2023-05-09 18 46 16](https://github.com/atsuyay/spring-gumball2/assets/60360870/28eb094e-9c0b-4b07-a99d-a9f7a3f9945c)
![スクリーンショット 2023-05-09 18 46 24](https://github.com/atsuyay/spring-gumball2/assets/60360870/bc31551a-3c82-43fb-a8da-5cdfb3b36779)
![スクリーンショット 2023-05-09 18 49 35](https://github.com/atsuyay/spring-gumball2/assets/60360870/b406883d-ba45-45e1-af2e-f8872e075177)
![スクリーンショット 2023-05-09 18 50 10](https://github.com/atsuyay/spring-gumball2/assets/60360870/f90036c8-deaf-4361-abbf-68dcdd9d96a0)
![スクリーンショット 2023-05-09 18 57 36](https://github.com/atsuyay/spring-gumball2/assets/60360870/da9c5368-a3e5-4cfb-9c38-788a4831c92c)
