### Hey, I'm Markus

Building from Finland on a 24 GB MacBook Pro.

Most of what I work on comes back to a few quiet questions: how does a finite mind hold onto exact truth across tens of thousands of steps without drifting? How should a reasoner rebuild its beliefs when a single premise underneath them changes? And how much real intelligence can actually live locally on your own desk instead of someone else's datacenter?

Right now I explore those through math, PyTorch experiments, and Apple Silicon MLX kernels:

| Experiment | The question behind it | Where it stands |
| :--- | :--- | :--- |
| **[wreath-deltanet](https://github.com/Manageriii/wreath-deltanet)** | Can `O(N)` linear attention keep exact state forever in `BF16` & `FP8` without losing GPU speed? | `100%` zero-shot `BF16` at `32,768` tokens (`682×` train length), `100%` `FP8` at `16K`, `6.3×` MPS chunk scan · [DOI](https://doi.org/10.5281/zenodo.24532887) |
| **[dflash-mlx-copyspec-benchmarks](https://github.com/Manageriii/dflash-mlx-copyspec-benchmarks)** | How fast can a 27B coding model actually think & write inside 24 GB of unified memory? | `70.98 tok/s` median on an M4 Pro via phase-aware `CopySpec` & EAGLE drafting (`<10.2 GB` active) |
| **[revisable-pyramid-reasoning](https://github.com/Manageriii/revisable-pyramid-reasoning)** | What happens when an AI tracks *why* it believes something and only rebuilds what broke? | ATMS taint-tracked revision + AST symbolic critics + `1.6×–2.0×` lossless MLX multi-token speculation |
| **[philosopher-micro-rsi](https://github.com/Manageriii/philosopher-micro-rsi)** | Can a tiny `1.52M` seed brain teach itself through parallel block diffusion and verified self-play? | `20.0% → 40.0%` verified Level-1 gain in 10 laptop sessions · Weights on [Hugging Face](https://huggingface.co/Manageriii/philosopher-micro-rsi) |

---

*Always happy to trade notes on linear attention, diffusion LMs, or Apple Silicon inference.*  
🤗 [huggingface.co/Manageriii](https://huggingface.co/Manageriii)
