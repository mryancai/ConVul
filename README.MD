# ConVul CVE dataset

This repository comprises a CVE dataset about concurrency vulnerabilities provided by ConVul, including:
  - UAF (Use After Free), 
  - NPD (Null Pointer Dereference), and 
  - DF (Double Free). 

We created this CVE dataset to evaluate ConVul's capability in detecting existing concurrency vulnerabilities. To achieve this, we searched the NVD vulnerability database, focusing on CVEs categorized under "Race" reported within the last decade (from 2008 to 2017). This results in 545 records. We then manually identified those caused by UAF, NPD, and DF, resulting in 82 CVEs. Following this, we excluded those on non-Linux platforms (i.e., on "Android", "Apple", "Java", "Windows kernel", and "Qualcomm") and those with no clear descriptions or without source and inputs (like POC). Finally, there are 10 CVEs left. We extracted the code involving vulnerabilities and also replaced non-Pthread synchronizations with Pthread ones. 

## Citing ConVul

ConVul has been accepted for publication at the 27th ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2019). If you use this dataset in your scientific work, please cite the paper as follows:

```
@inproceedings{convul,
  title={Detecting concurrency memory corruption vulnerabilities},
  author={Cai, Yan and Zhu, Biyun and Meng, Ruijie and Yun, Hao and He, Liang and Su, Purui and Liang, Bin},
  booktitle={Proceedings of the 2019 27th ACM Joint Meeting on European Software Engineering Conference and Symposium on the Foundations of Software Engineering},
  pages={706--717},
  year={2019}
}
```

## Questions

For any questions about this dataset or paper, please contact the corresponding author.

## License

This dataset is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.
