---
description: Steps to send data via delegate
---

# Delegate

### 1. Sender Side

* Create a protocol with method name in sender side. 

```swift
protocol ProtocolName {
    func functionName(parameter: Type)
}
```

* Create a delegate which adopts the protocol in the sender side.

```swift
var delegate: ProtocolName?
```

* Send the data via delegate by calling the methodName mentioned in the protocol in sender side.

```swift
delegate?.methodNameInProtocol(parameter: args)
```



### 2. Receiver Side

* Implement the protocol in the ViewController in the receiver end

```swift
Class ViewController: ProtocolName
```

* Enable receiving access in the receiver by creating an object 

```swift
var receiverObjectName = SenderClassName()
```

* Allow the delegate to report data to the receiver

```swift
receiverObjectName.delegate = self
```

* Access the methods mentioned in the protocol 

```swift
func functionName(parameters: DataType) {
    code here...
}
```

