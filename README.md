# SwiftSDK

This is a project for testing the creation of SDK and using with SPM (Swift Package Manager)

1 - Create a Swift / UIKit project and add the package

<img width="843" alt="image" src="https://github.com/lumana/SwiftSDK/assets/5826386/a80a94b9-c88a-4bda-9c01-cd0168f77896">


2- Import the SDK and use like this

    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view.
        
        let webView = SwiftSDK()
        self.view.addSubview(webView)
        
        webView.topAnchor.constraint(equalTo: view.topAnchor, constant: 0).isActive = true
        webView.bottomAnchor.constraint(equalTo: view.bottomAnchor, constant: 0).isActive = true
        webView.leadingAnchor.constraint(equalTo: view.leadingAnchor, constant: 0).isActive = true
        webView.trailingAnchor.constraint(equalTo: view.trailingAnchor, constant: 0).isActive = true
        webView.translatesAutoresizingMaskIntoConstraints = false
        
        webView.load()
    }


<img width="320" alt="image" src="https://github.com/lumana/SwiftSDK/assets/5826386/0309db36-d1f7-48d5-bcf0-56374edfeba0">
