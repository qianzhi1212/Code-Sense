# 练习 001：库存教学试跑

来源：2026-10-10 对话中的简化教学示例，无真实项目文件或 commit。用于测试学习流程，不作为真实商城完整实现。

## 需求与范围

实验业务约定：购买数量为正整数；不超过当前库存时购买成功并扣减，否则失败且库存不变。只讨论顺序调用和整数输入，其他项目能力未覆盖。这是本次整理明确写出的约定，不冒充试跑前已经完整固定的需求。

```java
public class Product {
    private int stock = 10;
    public boolean purchase(int quantity) {
        if (quantity <= stock) {
            stock = stock - quantity;
            return true;
        }
        return false;
    }
}
```

本题已讲解并暴露问题，只供回看与原题复判，不能再用于独立基线或未见迁移。
