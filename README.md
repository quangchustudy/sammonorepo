# MONOREPO CODEPIPLE WITH SAM PIPELINE AND LAMBDA


## I. Flow
[Link Reference](https://aws.amazon.com/blogs/compute/introducing-aws-sam-pipelines-automatically-generate-deployment-pipelines-for-serverless-applications/)

With modification for monorepo as below:
- Using monorepo template not normal template
- Setup the sub folder for each child lambda project in the monorepo
- Using the codepipeline for each child project
- Each commit to child project -> trigger the code pipeline for that project to run and deploy on 2 accounts (test and prod account)
- Trong monorepo có 2 child project dùng lambda là hello-sam-01 và hello-sam-02
- hello-sam-01 đã build pipeline bên trong -> hello-sam-02 build pipeline tương tự 01 với các thay đổi trong setting 
- khi commit các trên child project nào thì pipeline của child project đó sẽ chạy
- **Kiến trúc sử dụng các services để build phần pipeline này: TBU**

![The flow](images/Flow.png)

## I. Result

![Alt Text](images/result1.png)

![Alt Text](images/result2.png)

![Alt Text](images/result4.png)

![Alt Text](images/result3.png)
