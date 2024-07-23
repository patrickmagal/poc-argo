- kubectl argo rollouts get rollout rollouts-demo --watch

- kubectl argo rollouts set image rollouts-demo \
  rollouts-demo=argoproj/rollouts-demo:yellow

- kubectl argo rollouts promote rollouts-demo

- kubectl argo rollouts set image rollouts-demo \
  rollouts-demo=argoproj/rollouts-demo:red

- kubectl argo rollouts abort rollouts-demo
