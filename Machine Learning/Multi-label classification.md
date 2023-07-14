Multi label classification is used when there are multiple labels a given input could have and you need to predict which labels it does have and there probabilities. Unlike the softmax model where there can only be a single case for every input, multi label classification allows for multiple cases to be assigned to a single input. While you could train individual networks to find a given output probability of containing each label there is a better way to do it with multi label classification.

```mermaid
flowchart LR
    Input-.X--> L1 -.a^1--> L2 -.a^2--> a3(L3 of n labels) -.a^3-->id4(Output of n size with\n prob of each label)
```

The final layer in a multi label classification problem has a logistically [[Activation Functions|activated]] regression node for every possible label the input could have.