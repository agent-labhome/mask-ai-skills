# SKILL.md: Dog

## Core Functionality
**Dog** is a concise, no-frills file viewer that displays file contents directly to the terminal. It serves as a simpler alternative to `cat`, with syntax highlighting as its primary enhancement.

## Key Features
- **Syntax Highlighting**: Automatically applies color coding to source code and structured files based on file extension.
- **File Concatenation**: Can display multiple files sequentially in a single output stream.
- **Standard Input Support**: Reads from stdin when no filename is provided or when `-` is specified.
- **Minimalist Design**: Focuses on one job (viewing files) and does it well without complex options.

## Usage
```
dog [file...]
```
- View a single file: `dog README.md`
- View multiple files: `dog file1.txt file2.txt`
- Pipe input: `ls -la | dog`
- Use stdin explicitly: `dog -`

##"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":14,"completion_tokens":200,"total_tokens":214,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":14},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache