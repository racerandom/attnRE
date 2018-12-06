# attention-based relation classification


##SemEval2010_task8

|Models|attention|score|pre-trained|position feats|freeze embed|monitor|batch size| official macro-F1| random search|
|------|---------|-----|-----------|---------------|------------|-------|----------|------------------|--------------|
|entiAttnMatRNN|entity-wise|weight matrix|glove.d100|none|FALSE|val_acc|32| 81.43% |200|
|attnMatRNN|last hidden|weight matrix|glove.d100|PI|FALSE|val_acc|32| 80.93%|200|
|attnMatRNN|last hidden|weight matrix|glove.d100|none|FALSE|val_acc|32| 68.83%|200|
|attnRNN(baseline)|all hidden|weight vector|glove.d100|PI|FALSE|val_acc|32| 80.59%|200|
|attnRNN(baseline)|all hidden|weight vector|glove.d100|none|FALSE|val_acc|32|70.90% |200|

