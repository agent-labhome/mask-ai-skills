# SKILL.md: Mobile App Development

## Metadata
- **Skill Category**: Technical Development
- **Proficiency Levels**: Beginner → Intermediate → Advanced → Expert
- **Time to Basic Proficiency**: 3-6 months
- **Time to Advanced Proficiency**: 2-3 years
- **Related Skills**: UI/UX Design, Backend Development, Product Management, QA Testing
- **Tools Ecosystem**: IDEs, Frameworks, Testing Suites, Deployment Platforms

## Practical Skill Components

### 1. Core Competencies

#### Platform-Specific Development
**iOS (Swift/SwiftUI)**
```swift
// Example: Basic SwiftUI view
struct ContentView: View {
    @State private var count = 0
    
    var body: some View {
        VStack {
            Text(\"Count: \(count)\")
                .font(.title)
            Button(\"Increment\") {
                count += 1
            }
            .buttonStyle(.borderedProminent)
        }
        .padding()
    }
}
```

**Android (Kotlin/Jetpack Compose)**
```kotlin
// Example: Basic Composable function
@Composable
fun CounterScreen() {
    var count by remember { mutableStateOf(0) }
    
    Column(
        modifier = Modifier.padding(16.dp),
        horizontalAlignment = Alignment.CenterHorizontally
    ) {
        Text(
            text = \""},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":18,"completion_tokens":300,"total_tokens":318,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":18},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
