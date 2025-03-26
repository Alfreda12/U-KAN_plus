# U-KAN_plus

### Training U-KAN_plus

You can simply train U-KAN_plus on a single GPU by specifing the dataset name ```--dataset``` and input size ```--input_size```.

```bash
python train.py --arch UKAN_plus --dataset ${dataset} --input_w ${input_size} --input_h ${input_size} --name ${dataset}_UKAN_plus  --data_dir [YOUR_DATA_DIR]
```

For example, train U-KAN_plus with the resolution of 256x256 with a single GPU on the BUSI dataset in the ```inputs``` dir:

```bash
python train.py --arch UKAN_plus --dataset busi --input_w 256 --input_h 256 --name busi_UKAN_plus  --data_dir ./inputs
```

### Evaluating U-KAN_plus

You can evaluate U-KAN_plus using the following code

```bash
python val.py --name ${dataset}_UKAN_plus --output_dir [YOUR_OUTPUT_DIR] 
```

For example

```bash
python val.py --name busi_UKAN_plus --output_dir outputs
```

