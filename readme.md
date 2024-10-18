# Code for "Getting in the Door: Streamlining Intake in Civil Legal Services with Large Language Models"

This repository contains the code for the paper "Getting in the Door: Streamlining Intake in Civil Legal Services with Large Language Models", available at:
[https://arxiv.org/abs/2410.03762](https://arxiv.org/abs/2410.03762), and accepted at JURIX 2024.

The code in notebook.ipynb loads a number of scenarios (from scenarios.tsv) and intake rules (intake_J1.txt, intake_J2.txt, intake_J3.txt), and then uses various LLMs to predict whether a certain factual situation falls under the provided intake rules. The results are exported to a file that can be further analyzed.

To run this project, you need to provide your own LLM API keys. To do so, copy the .env-example into .env, and add the keys for the models you want to use.
Then, set up a new python environment, install the requirements.txt file, and start a jupyter notebook server to run notebook.ipynb.

If you use the code, please cite us at:
```
@misc{steenhuis2024gettingdoorstreamliningintake,
      title={Getting in the Door: Streamlining Intake in Civil Legal Services with Large Language Models}, 
      author={Quinten Steenhuis and Hannes Westermann},
      year={2024},
      eprint={2410.03762},
      archivePrefix={arXiv},
      primaryClass={cs.HC},
      url={https://arxiv.org/abs/2410.03762}, 
}
```

# Paper Abstract:
Legal intake, the process of finding out if an applicant is eligible for help from a free legal aid program, takes significant time and resources. In part this is because eligibility criteria are nuanced, open-textured, and require frequent revision as grants start and end. In this paper, we investigate the use of large language models (LLMs) to reduce this burden. We describe a digital intake platform that combines logical rules with LLMs to offer eligibility recommendations, and we evaluate the ability of 8 different LLMs to perform this task. We find promising results for this approach to help close the access to justice gap, with the best model reaching an F1 score of .82, while minimizing false negatives.