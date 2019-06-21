```
.Total configs: 2
Testing config 32x32
Downloading and preparing dataset downsampled_imagenet (?? GiB) to /tmp/downsampled_imagenet_testwyr326xt/tmplxjpw1r9/downsampled_imagenet/32x32/0.1.0...
E..s
======================================================================
ERROR: test_download_and_prepare_as_dataset (__main__.DownsampledImagenetTest)
test_download_and_prepare_as_dataset (__main__.DownsampledImagenetTest)
Run the decorated test method.
----------------------------------------------------------------------
Traceback (most recent call last):
  File "/home/chanchal/anaconda3/lib/python3.6/site-packages/tensorflow_datasets/testing/test_utils.py", line 185, in decorated
    f(self, *args, **kwargs)
  File "/home/chanchal/anaconda3/lib/python3.6/site-packages/tensorflow_datasets/testing/dataset_builder_testing.py", line 213, in test_download_and_prepare_as_dataset
    self._download_and_prepare_as_dataset(builder)
  File "/home/chanchal/anaconda3/lib/python3.6/site-packages/tensorflow_datasets/testing/dataset_builder_testing.py", line 247, in _download_and_prepare_as_dataset
    builder.download_and_prepare(download_config=download_config)
  File "/home/chanchal/anaconda3/lib/python3.6/site-packages/tensorflow_datasets/core/api_utils.py", line 52, in disallow_positional_args_dec
    return fn(*args, **kwargs)
  File "/home/chanchal/anaconda3/lib/python3.6/site-packages/tensorflow_datasets/core/dataset_builder.py", line 285, in download_and_prepare
    download_config=download_config)
  File "/home/chanchal/anaconda3/lib/python3.6/site-packages/tensorflow_datasets/core/dataset_builder.py", line 816, in _download_and_prepare
    max_examples_per_split=download_config.max_examples_per_split,
  File "/home/chanchal/anaconda3/lib/python3.6/site-packages/tensorflow_datasets/core/dataset_builder.py", line 694, in _download_and_prepare
    self._prepare_split(split_generator, **prepare_split_kwargs)
  File "/home/chanchal/anaconda3/lib/python3.6/site-packages/tensorflow_datasets/core/dataset_builder.py", line 820, in _prepare_split
    generator = self._generate_examples(**split_generator.gen_kwargs)
  File "/home/chanchal/anaconda3/lib/python3.6/site-packages/tensorflow_datasets/image/downsampled_imagenet.py", line 128, in _generate_examples
    for fname, fobj in archive:
  File "/home/chanchal/anaconda3/lib/python3.6/site-packages/tensorflow_datasets/core/download/extractor.py", line 149, in iter_tar
    tar = tarfile.open(mode=read_type, fileobj=fobj)
  File "/home/chanchal/anaconda3/lib/python3.6/tarfile.py", line 1574, in open
    raise ReadError("file could not be opened successfully")
tarfile.ReadError: file could not be opened successfully

----------------------------------------------------------------------
Ran 5 tests in 0.268s

FAILED (errors=1, skipped=1)
```
