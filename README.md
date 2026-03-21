<div align="center">

# مكتبة GPU للغة المرجع
### Al-Marjaa GPU Library

[![Version](https://img.shields.io/badge/version-3.4.0-blue.svg)](https://github.com/radhwendalyhamdouni/Al-Marjaa-GPU)

**المخترع والمطور: رضوان دالي حمدوني**

</div>

---

## 🎯 نظرة عامة

مكتبة GPU Computing للغة المرجع - CUDA, OpenCL.

---

## 📦 التثبيت

```toml
[dependencies]
almarjaa-gpu = { git = "https://github.com/radhwendalyhamdouni/Al-Marjaa-GPU" }
```

---

## 💡 مثال الاستخدام

```rust
use almarjaa_gpu::{GpuEngine, ComputeKernel};

fn main() -> Result<(), Box<dyn std::error::Error>> {
    let gpu = GpuEngine::new()?;
    let kernel = gpu.load_kernel("compute.cu")?;
    let result = kernel.execute(&data)?;
    Ok(())
}
```

---

**صُنع بـ ❤️ للعالم العربي**
