<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-typesafe-ai 1.3.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-typesafe-ai.git", from: "1.3.0")
```

Products: `SwiftAITypeSafeAI`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# TypeSafe AI for Swift

`SwiftAITypeSafeAI` adds TypeSafe AI to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/typesafe-ai` and supports evaluation and decisions.

Provider guide with models, options, streaming and errors:

- [TypeSafe AI](https://swiftaisdk.github.io/SwiftAISDK/providers/typesafe/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAITypeSafeAI` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAITypeSafeAI

let provider = try AIProviders.typeSafeAI(configuration: TypeSafeAIProviderSettings())
```

By default the provider reads `TYPESAFE_AI_API_KEY` from the environment; values set in `TypeSafeAIProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-typesafe-ai` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.
