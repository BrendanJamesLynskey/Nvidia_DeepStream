# NVIDIA DeepStream &mdash; Presentation Series

A comprehensive, high-quality, eight-part visual presentation on **NVIDIA DeepStream** &mdash; the streaming vision-AI SDK for building hardware-accelerated video-analytics pipelines on Jetson and dGPU. Presented for engineers: every deck answers *what problem it solves*, *how the mechanism works*, and *why it matters when you build and operate real systems*, with hand-drawn SVG diagrams throughout.

**Live index:** https://brendanjameslynskey.github.io/Nvidia_DeepStream/

## Presentations in this series

| # | Title | Status | What it covers |
|---|-------|--------|----------------|
| 01 | [The Big Picture](https://brendanjameslynskey.github.io/Nvidia_DeepStream/part1.html) | live | What DeepStream is and why it exists &mdash; turning many live streams into real-time structured insight, accelerated end-to-end on NVIDIA. The canonical pipeline, the software stack, where it runs (Jetson to dGPU), and its use cases. |
| 02 | [GStreamer Foundations &amp; the DeepStream Architecture](https://brendanjameslynskey.github.io/Nvidia_DeepStream/part2.html) | live | DeepStream as a set of accelerated GStreamer plugins &mdash; elements, pads, caps negotiation and buffers; the NVDEC / NVENC / GPU / VIC / DLA hardware blocks; and the zero-copy NVMM / NvBufSurface memory model. |
| 03 | [The Plugin Toolbox](https://brendanjameslynskey.github.io/Nvidia_DeepStream/part3.html) | live | A tour of the 40+ plugins by role &mdash; input &amp; decode, batching &amp; routing (nvstreammux / nvstreamdemux), inference, analytics &amp; CV, compositing &amp; OSD, output &amp; messaging &mdash; mapped onto the reference pipeline. |
| 04 | [Inference &mdash; nvinfer, TensorRT &amp; Triton](https://brendanjameslynskey.github.io/Nvidia_DeepStream/part4.html) | live | Primary vs secondary GIE; building and caching TensorRT engines; the config-file anatomy; pre-processing, clustering and custom parsers; batching and interval; Triton via nvinferserver; and TAO pretrained models. |
| 05 | [Multi-Object Tracking](https://brendanjameslynskey.github.io/Nvidia_DeepStream/part5.html) | live | Persistent identity across frames with nvtracker and the composable NvMultiObjectTracker library &mdash; IOU, NvSORT, NvDCF and NvDeepSORT; Re-ID galleries and re-association; the YAML config; and single-view 3D tracking. |
| 06 | [Metadata &amp; Analytics](https://brendanjameslynskey.github.io/Nvidia_DeepStream/part6.html) | live | The NvDsBatchMeta &rarr; frame &rarr; object &rarr; classifier hierarchy; metadata pools and lifecycle; reading it in buffer probes (C and pyds); extending it with user meta; and the nvdsanalytics rule engine. |
| 07 | [Messaging, Smart Record &amp; IoT](https://brendanjameslynskey.github.io/Nvidia_DeepStream/part7.html) | live | The last mile &mdash; nvmsgconv serialising events to JSON / protobuf, nvmsgbroker shipping to Kafka / MQTT / AMQP / Azure IoT / Redis; smart-record event clips; bidirectional cloud-to-edge control; and the REST API for dynamic streams. |
| 08 | [Building &amp; Deploying](https://brendanjameslynskey.github.io/Nvidia_DeepStream/part8.html) | live | Four ways to build &mdash; config-driven deepstream-app, C/C++, Python (pyds), and Graph Composer / Service Maker; packaging with NGC, JetPack and Kubernetes; and performance tuning for maximum streams-per-GPU. |

## How to read this series

The eight decks are ordered to build on one another. **Part 01** gives the big picture and **Part 02** the GStreamer and on-GPU memory foundation that everything else assumes. **Parts 03&ndash;07** each take one subsystem &mdash; the plugin set, inference, tracking, the metadata graph, and messaging &mdash; and go deep. **Part 08** pulls it together into how you actually build, containerise and tune a production pipeline. Each deck also stands alone, so if you already know GStreamer you can jump straight to the subsystem you need.

## Where this fits

Part of the [LLMs hub](https://github.com/BrendanJamesLynskey/LLMs) &mdash; an index of presentation series for AI / LLM / vision-AI engineers &mdash; under **Hardware &amp; Inference**. Complements the [NVIDIA GPU Architectures](https://github.com/BrendanJamesLynskey/LLM_Hub_NVIDIA_GPUs), [CUDA Programming](https://github.com/BrendanJamesLynskey/LLM_Hub_CUDA) and [Vision-Language Models](https://github.com/BrendanJamesLynskey/LLM_Hub_Vision_Language) series: DeepStream is where trained vision models are put to work as real-time, hardware-accelerated streaming pipelines.

Source material throughout is the [NVIDIA DeepStream documentation](https://docs.nvidia.com/metropolis/deepstream/dev-guide/). DeepStream is part of the [NVIDIA Metropolis](https://developer.nvidia.com/metropolis) application framework.

---

*Interactive HTML decks rendered on GitHub Pages. No build step &mdash; each part is a single self-contained `.html` file.*
