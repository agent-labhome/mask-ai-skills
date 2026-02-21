# Unreal Engine SKILL.md

## Metadata
- **Category**: Game Development / Real-time 3D Creation
- **Prerequisites**: Basic programming knowledge (C++ preferred), 3D math fundamentals
- **Difficulty**: Intermediate to Advanced
- **Time Investment**: 6-12 months for proficiency
- **Key Tools**: Unreal Editor, Blueprints Visual Scripting, C++, Marketplace, Quixel Bridge
- **Latest Version**: Unreal Engine 5.3+ (as of 2024)

## Core Competencies

### 1. **Editor Proficiency**
- **Navigation**: Viewport controls, content browser organization, world outliner management
- **Level Design**: BSP geometry, landscape tools, foliage painting, world composition
- **Asset Management**: Import/export pipelines, material/texture organization, asset referencing

### 2. **Blueprints Visual Scripting**
- **Essential Nodes**: Variables, functions, events, flow control, timelines
- **Common Systems**: 
  - Character controllers and input handling
  - UI widgets and HUD creation
  - Game state management
  - AI behavior trees and blackboards
- **Best Practices**: 
  - Use macros for reusable logic
  - Implement interfaces for communication
  - Organize with comment boxes and reroute nodes
  - Avoid deep nesting (use functions)

### 3. **C++ Programming**
- **Core Concepts**:
  ```cpp
  // Basic Actor class
  UCLASS()
  class AMYCharacter : public ACharacter
  {
      GENERATED_BODY()
      
      UPROPERTY(EditAnywhere, BlueprintReadWrite)
      float Health = 100.0f;
      
      UFUNCTION(BlueprintCallable)
      void TakeDamage(float DamageAmount);
  };
  ```
- **Key Areas**:
  - Gameplay framework classes (Actor, Pawn, Character, Controller)
  - UPROPERTY and UFUNCTION specifiers
  - Delegates and events
  - Plugin development

### 4. **Materials and Shaders**
- **Material Editor**: Master materials, material instances, parameter collections
- **Essential Techniques**"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":19,"completion_tokens":450,"total_tokens":469,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":19},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
