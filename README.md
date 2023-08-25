# olive-exercises
A couple Python scripts and (input) model configs for Microsoft's [Olive tool](https://github.com/microsoft/Olive)

## Installation

Install all dependencies listed in `requirements.txt` and `additional_requirements.txt`
by running:
```python
pip install -r requirements.txt
pip install -r additional_requirements.txt
```

## Running a ResNet PTQ (CPU) Example

Prepare the data and model by running the following script:
`python prepare_model_data.py`

```python
python -m olive.workflows.run --config resnet_ptq_cpu.json --setup
```

```python
python -m olive.workflows.run --config resnet_ptq_cpu.json
```

NOTE:
The `resnet_ptq_cpu.json`, `user_script.py` and `prepare_model_data.py` source
files are provided in the [Olive GitHub repository](https://github.com/microsoft/Olive/tree/main/examples/resnet)


### File Structure

- `sample_output` - This directory contains `.txt` files of sample optimization
pass outputs
