# BLS-Location-System
The code is for paper "BLS-Location: A Wireless Fingerprint Localization Algorithm Based on Broad Learning".

If you use this work for your research, you may want to cite

```
@article{zhu2021bls,
  title={{BLS-Location: A Wireless Fingerprint Localization Algorithm Based on Broad Learning}},
  author={Zhu, Xiaoqiang and Qiu, Tie and Qu, Wenyu and Zhou, Xiaobo and Atiquzzaman, Mohammed and Wu, Dapeng},
  journal={IEEE Transactions on Mobile Computing},
  volume={22},
  number={1},
  pages={115--128},
  year={2023}
}
```

### Prepare the datasets:
Download the data: 
```
git clone https://github.com/qiang5love1314/CSI-dataset.git
```
Move the data into the root folder:
```
cd CSI-dataset/Meeting
find ./ -name "coordinate*.mat" -print0 | xargs -0 mv -t ./
```

### Run and get the results:
```
python MeetingMain.py
```

#### Modify the \# of antennas
Find the line with comments with \# antennas, e.g, `# 3 antennas`
Uncomment all the lines and comment others and run the code. Current default is 3 antennas. 
