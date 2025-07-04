# Continous delivery vs Continous Deployment

![alt text](image-4.png)

- Delivery : more manual labour
- Deployment : more automated tasks
  ![alt text](image.png)
  ![alt text](image-3.png)
- Blue-green Deployment -> keep app in prod and create new version for Deployment -> route to new version
- ![alt text](image-1.png)
- Canary Deployment -> update servers one-by-one -> you add one new server and push some users to that new server, if no bugs update another server etc
- ![alt text](image-2.png)

## Continous Testing

- process of executing automated taests as part of the delivery pipeline
- Smoke test, rest test
- ![alt text](image-5.png)
- ![alt text](image-6.png)
- ![alt text](image-7.png)
- ![alt text](image-8.png)

## Infrastructure as a Code - Terraform

- Terraform is a tool for IaC
- used to maintain standardized code??
- ![alt text](image-9.png)
- ![alt text](image-10.png)
- ![alt text](image-11.png)

## Configuration Management

- managing and changing the state of pieces of infrastructure in a consistent and maintainable way
- CM ttols are a great way to implement IaC
- Tools to maintain configuration of data -> ansible, puppet, chef, salt
- ![alt text](image-12.png)

## Containerization

- Convert apps to run inside a container
- Convert Monolithic to microservices
- Done by developers
- ![alt text](image-13.png)
- ![alt text](image-14.png)
- ![alt text](image-15.png)
- ![alt text](image-16.png)
- ![alt text](image-17.png)

## Security Development Lifecycle

1. Training - security training
   ![alt text](image-19.png)
2. Requirements - establish security requirement
   ![alt text](image-20.png)
3. Design - establish design requirements and analyse attack surface
   ![alt text](image-21.png)
4. Implementation - use approved/enterprise tools -> remove/delete unsafe functions
   ![alt text](image-22.png)
5. Verification -> verify no security leak -> review attack surface established when designing
   ![alt text](image-23.png)
6. Release -> establish incident response plan -> conduct final security review
   ![alt text](image-24.png)
7. Response ->

![alt text](image-18.png)
