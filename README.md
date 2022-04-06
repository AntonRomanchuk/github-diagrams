```mermaid
sequenceDiagram
    participant View
    participant Presenter
    participant Model

    View->>Presenter: viewDidLoad
    Presenter->>View: showActivity
    Presenter->>Model: requestProduct
    Model->>Presenter: didLoad
    Presenter->>View: hideActivity
    Presenter->>View: refresh
```
