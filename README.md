# VSA project repo

## Introduction


A Video Search Assistant (VSA) is an application allowing users to apply AI to search videos for scenes of interest in videos (e.g., movie, clips from Vimeo or TikTok, other).
Imagine an index at the end of a textbook where the reader can identify pages where certain ideas and concepts may be found.
Now, generalize this index to a video application.

The application is provided video input and analyzes the multimedia content.
Once analyzed for specific characteristics (e.g., times in the video when certain actor is present and/or conducting a certain action), the metadata is loaded into a database / search engine (e.g., Elasticsearch or Algolia) where users can identify the time stamp of scene of interest through a web browser user interface.
The time stamp informs users where to easily navigate to find the desired people, activities, etc. that was queried of the video.

Many AI-enabled methods and tools are supposed to perform classification analysis across these different data streams.
The video search assistant may use any data stream type classification strategy, or implement a solution that combine more than one strategy.

# Milestone 0: Prepare materials
- Setup Jetson Nano
  - [X] Connecting Network with VPN
  - [X] Setting CSI Camera
  
- Installation Deepstream sdk
  - [X] pull docker image
  
- Setup search system
  - [X] Create AWS OpenSearch instance

# Milestone 1: Simple VSA and Jetson Nano Orientation
- Jetson Nano Orientation
    - [X] Nvidia DLI Course
    - [X] Experiments with Nvidia examples

- Framework Selection for model training
  - Action recognition: Deepstream SDK, Resnet18-2D/3D(ActionRecognitionNet from Nvidia NGC)
  - Face recognition: Pytorch(ONNX), MTCNN(for Detection), InceptionResnetV1(for Verification)

- Setup Jetson Nano
    - [X] Setup streaming video with RTSP

# Milestone 2: Transfer Learning & Inference
- Transfer learning
  - Action recognition
    - [X] Nvidia TAO toolkit
  - Face recognition
    - [X] Pytorch implementation

- Inference
    - [X] Action recognition: using Deepstream 
    - [X] Face recognition: using TensorRT

# Milestone 3(Final)
- Complete pipelines
- Link to Opensearch system
- Make demonstrations
