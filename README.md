# Step-by-Step Reasoning to Solve Grid Puzzles: Where do LLMs Falter?
Solving grid puzzles involves a significant amount of logical reasoning. Hence, it is a good domain to evaluate the reasoning capability of a model which can then guide us to improve the reasoning ability of models. However, most existing works evaluate only the final predicted answer of a puzzle, without delving into an in-depth analysis of the LLMs' reasoning chains (such as where they falter) or providing any finer metrics to evaluate them. Since LLMs may rely on simple heuristics or artifacts to predict the final answer, it is crucial to evaluate the generated reasoning chain beyond overall correctness measures, for accurately evaluating the reasoning abilities of LLMs. To this end, we first develop GridPuzzle, an evaluation dataset comprising 274 grid-based puzzles with different complexities. Second, we propose a new error taxonomy derived from manual analysis of reasoning chains from LLMs including GPT-4, Claude-3, Gemini, Mistral, and Llama-2. Then, we develop an LLM-based framework for large-scale subjective evaluation (i.e., identifying errors) and an objective metric, PuzzleEval, to evaluate the correctness of reasoning chains. Evaluating reasoning chains from LLMs leads to several interesting findings. We further show that existing prompting methods used for enhancing models' reasoning abilities do not improve performance on GridPuzzle. This highlights the importance of understanding fine-grained errors and presents a challenge for future research to enhance LLMs' puzzle-solving abilities by developing methods that address these errors.
 
![puzzleteaser](https://github.com/Mihir3009/GridPuzzle/assets/55184768/9dcb41af-6fa9-45e5-bf04-f4121e851018)

## Data Release
Please take a look at the ./data folder to access the GridPuzzle dataset and the data for all the experiments.
<br><br>
Scope of the dataset: The dataset consists of GridPuzzle with the original reasoning chains, the data for Auto-evaluation done by GPT-4o, the data for both the Metrics, Accuracy and PuzzleEval, and finally the data for the Mitigation strategies.
<br> 
The ```data/``` folder contains the following files:  
    
    ├── ...
    ├── data/
      ├── GridPuzzle
      ├── Auto-Evaluation
      ├── Metrics
      │   ├── Accuracy
      │   └── PuzzleEval
      └── Mitigation
          ├── Mitigation Results
          └── PuzzleEval Results

## Excel File format for GridPuzzle


## Excel File format for Auto-Evaluation

## Excel File format for Accuracy

## Excel File format for PuzzleEval
