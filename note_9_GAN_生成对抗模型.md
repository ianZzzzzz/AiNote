```mermaid
graph TB
    随机噪声 
    Generator
    伪造品
    真品
    object
    Discriminator
    真实
   

    随机噪声 --输入--> Generator --制造--> 伪造品 --> object
    
    真品 --> object
   
    
    object-->label
    object-->Discriminator --score-->loss_function
    label-->loss_function-->optimizer-->Discriminator


```
```mermaid
graph TB
    
```