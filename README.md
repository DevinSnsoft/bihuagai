环境：
python>3.6
pytorch (>=1.5)
* sconf, numpy, scipy, scikit-image, tqdm, jsonlib, fonttools


data:
./data

ttf转txt：
在文件夹中放置TTF文档，运行：
python ttf2txt.py --path
可以自由分配组件


准备数据（不自由分配）：
python get_chars_from_ttf.py --root_dir path/to/ttf/dir

run train:
python train.py cfgs/train.yaml

run test:
python eval.py \
    cfgs/eval.yaml \
    --weight generator.pth \
    --result_dir path/to/save/images










