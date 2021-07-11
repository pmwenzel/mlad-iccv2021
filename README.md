# MLAD ICCV 2021 Localization Challenge

For the localization challenge, we provide three different scenarios, each consisting of a reference map and a query sequence from the [4Seasons](https://www.4seasons-dataset.com/) dataset. 

1. Countryside
  * reference map: `recording_2020-10-08_09-57-28`
  * query sequence: `recording_2021-01-07_14-03-57`
2. Old Town
  * reference map: `recording_2020-10-08_11-53-41`
  * query sequence: `recording_2021-05-10_19-51-14`
3. Neighborhood
  * reference map: `recording_2021-02-25_13-25-15`
  * query sequence: `recording_2021-05-10_18-26-26`

Each reference map contains highly accurate reference poses. All sequences from the [4Seasons](https://www.4seasons-dataset.com/) dataset can be used as training data.

## Dataset Download

To download the challenge data and other sequences from the dataset, we refer to the [download](https://www.4seasons-dataset.com/dataset) page.

## Dataset Structure

For details on the dataset structure, we refer to the following [documentation](https://www.4seasons-dataset.com/documentation).

## Libartipy Python Library

In this [repository](https://github.com/Artisense-ai/libartipy), you will find a set of tools for working with the 4Seasons dataset.

## Task

Each `relocalizationFile_recording_source_to_recording_target.txt` contains a list of first the keyframe from the source (reference) sequence and the query keyframe. The task is to provide the relative pose between the source and the query frame. Note that the relative pose is from cam0 of the reference sequence to cam0 of the query sequence, respectively. The `6DOF` poses are specified as translation (`t_x`, `t_y`, `t_z`), and quaternion (`q_x`, `q_y`, `q_z`, `q_w`).

## Submission

For the test sequences, the ground truth is withheld. For submitting your results to the challenge, please refer to the steps described at: [https://sites.google.com/view/mlad-iccv2021/challenge](https://sites.google.com/view/mlad-iccv2021/challenge).