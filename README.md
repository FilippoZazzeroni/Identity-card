# Identity Card

Identity Card is an app that let you idenity your self with the new governament scheme. It complies with all the European and American rules of identification.
The code is pretty simple and straightforeward beacuse it has to be understood immediatly.

```
  //
  //  ViewController.swift
  //  identity_card
  //
  //  Created by Filippo Zazzeroni on 15/06/22.
  //
  import UIKit

  class ViewController: UIViewController {

      @IBOutlet private weak var label: UILabel!

      @IBOutlet private weak var surname: UITextField!

      @IBOutlet private weak var name: UITextField!

      //

      override func viewDidLoad() {
          super.viewDidLoad()
          label.isHidden = true
      }

      @IBAction func checkIdentity(_ sender: Any) {
          onCheckIdentiyPressed(from: "Filippo Zazzeroni")
      }

      private func onCheckIdentiyPressed(from filippo: String) {
          label.text = "Si"
          label.isHidden = false
      }


  }
```
