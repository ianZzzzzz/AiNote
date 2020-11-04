```mermaid
graph TB
    随机噪声 
    Generator
    伪造品
    真品
    object
    Discriminator
    
   

    随机噪声 --输入--> Generator --制造--> 伪造品 --> object
    
    真品 --> object
   
    
    object-->label
    object-->Discriminator -->D_loss_function
    label-->D_loss_function-->optimizer-->Discriminator
    Discriminator-->G_loss_function-->Generator


```
```mermaid
graph TB
    
```