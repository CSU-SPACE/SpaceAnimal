# SpaceAnimal Evaluation Tools

## Installation
1. Clone the repository
```
git clone https://github.com/CSU-SPACE/SpaceAnimal.git
```
2. Install the requirements
```
cd SpaceAnimal/eval_tools
pip install -r requirements.txt
```

## Pose Tracking Evaluation
Test command with example data:
```
python eval_tools/evalpose/evaluate.py \
-g eval_tools/examples/posetrack_gts/ \
-p eval_tools/examples/posetrack_preds/ \
-c worm
-o eval_tools/out
```

## Acknowledgement
This work is built on top of the [poseval](https://github.com/leonid-pishchulin/poseval) repository by Leonid Pishchulin.