Mermaid - https://github.com/mermaid-js/mermaid
Live editor - https://mermaid-js.github.io/mermaid-live-editor/edit
Confluence example - https://toshihiro.atlassian.net/wiki/spaces/MIFC/pages/338984978/Demo

https://wiki.shop-apotheke.com/display/MAPPD/MVP+-+Model+View+Presenter

```mermaid
graph TD
    A[Presenter] -->|Update model| C[Model]
    C -->|Model changed| A
    B[View] -->|User actions| A
    A -->|Update UI| B
```

<details>
  <summary>Code</summary>
 
  ```
  graph TD
    A[Presenter] -->|Update model| C[Model]
    C -->|Model changed| A
    B[View] -->|User actions| A
    A -->|Update UI| B
  ```
  
</details>

```mermaid
sequenceDiagram
    participant View
    participant Presenter
    participant Model

    View->>Presenter: viewDidLoad
    Presenter-->>View: showActivity
    Presenter->>Model: requestProduct
    Model->>Presenter: didLoad
    Presenter-->>View: hideActivity
    Presenter->>View: refresh
```

<details>
  <summary>Code</summary>
 
  ```
  sequenceDiagram
    participant View
    participant Presenter
    participant Model

    View->>Presenter: viewDidLoad
    Presenter-->>View: showActivity
    Presenter->>Model: requestProduct
    Model->>Presenter: didLoad
    Presenter-->>View: hideActivity
    Presenter->>View: refresh
  ```
  
</details>

https://wiki.shop-apotheke.com/display/MAPPD/iOS+Singletons+Refactoring

```mermaid
classDiagram
    XS_Shop <|-- SAE_ViewController : Some hint
    XS_Shop <|-- SAE_CartVoucherAreaTvCellModel
    XS_Shop <|-- XS_Address
    XS_Shop <|-- XS_Settings
    XS_Shop : +singleton
    XS_Shop : -shopConfiguration
    XS_Shop: -login()
    XS_Shop: -requestFromNetwork()

    class SAE_ViewController {
      Base ViewController
    }

    class SAE_CartVoucherAreaTvCellModel {
      Cell configurator
    }
    
    class XS_Address {
      Model
    }

    class XS_Settings {
      Also singleton
    }
```

<details>
  <summary>Code</summary>
 
  ```
classDiagram
    XS_Shop <|-- SAE_ViewController : Some hint
    XS_Shop <|-- SAE_CartVoucherAreaTvCellModel
    XS_Shop <|-- XS_Address
    XS_Shop <|-- XS_Settings
    XS_Shop : +singleton
    XS_Shop : -shopConfiguration
    XS_Shop: -login()
    XS_Shop: -requestFromNetwork()

    class SAE_ViewController {
      Base ViewController
    }

    class SAE_CartVoucherAreaTvCellModel {
      Cell configurator
    }
    
    class XS_Address {
      Model
    }

    class XS_Settings {
      Also singleton
    }
  ```
  
</details>

Our accessibility data

```mermaid
pie title Font size
    "A11y_M" : 2248
    "A11y_L" : 842
    "A11y_XL" : 9.07
    "XXL" : 176
    "A11y_XXL" : 41
    "A11y_XXXL" : 25
    "XS" : 9183
    "S" : 6965
    "M" : 14216
    "Default" : 169107
    "XL" : 24372
    "XXL" : 17077
    "XXXL" : 24373   
```

<details>
  <summary>Code</summary>
 
  ```
pie title Font size
    "A11y_M" : 2248
    "A11y_L" : 842
    "A11y_XL" : 9.07
    "XXL" : 176
    "A11y_XXL" : 41
    "A11y_XXXL" : 25
    "XS" : 9183
    "S" : 6965
    "M" : 14216
    "Default" : 169107
    "XL" : 24372
    "XXL" : 17077
    "XXXL" : 24373   
  ```
  
</details>
