# Dynamic Min_DF Optimization for Text Summarization

## Overview

This repository contains the implementation of a dynamic optimization approach for the `min_df` parameter in text summarization tasks, as described in the study "The Devil is in the details: GreedSum optimization for minimum document frequency." The primary goal of this implementation is to enhance the quality of extractive text summarization by optimizing the `min_df` parameter to achieve the best possible ROUGE scores, a standard benchmark for summarization quality.

## Description

The code within this repository is designed to dynamically adjust the `min_df` parameter, which specifies the minimum document frequency of words to be considered in the summarization process. Unlike static approaches, this dynamic method tailors the `min_df` setting for each individual text, aiming to optimize the balance between including informative words and excluding less relevant ones. The optimization process seeks to identify the `min_df` value that yields the highest ROUGE score, indicating the most effective summarization performance for each document.

## How It Works

The implementation follows a systematic approach to optimize the `min_df` parameter:

1. **Data Processing:** Initially, the text data is preprocessed to suit the needs of summarization, setting the stage for the optimization process.
2. **Optimization Routine:** The core of the script dynamically adjusts the `min_df` parameter across different values, evaluating the impact of each adjustment on the summarization quality through ROUGE scores.
3. **Evaluation:** The optimal `min_df` setting is determined by the value that results in the highest ROUGE score, indicating the most accurate and concise summarization of the text.

## Usage

To utilize this optimization framework in your text summarization projects, follow these steps:

1. **Prepare Your Dataset:** Download the dataset from the corresponding links : Full dataset with 17038 article texts   https://data.mendeley.com/datasets/nvsxfcbzdk/2 , Sample of 376 article texts - https://data.mendeley.com/datasets/6zx6fw5t4t/1.
2. **Run the Optimization:** Execute the script to start the dynamic optimization process. The script will iterate through various `min_df` values, evaluate their efficacy using ROUGE scores, and identify the most optimal setting.
3. **Review Results:** The final output will include the optimal `min_df` value for your dataset, along with the corresponding ROUGE score, indicating the effectiveness of the summarization.

## Contributing

Your contributions are welcome! Whether you're fixing bugs, improving the documentation, or proposing new features, we appreciate your interest in enhancing this dynamic optimization tool.


## Acknowledgments

This work is inspired by the research detailed in "The Devil is in the details: GreedSum optimization for minimum document frequency," focusing on improving the precision of extractive text summarization through dynamic parameter optimization. 
