# attention-based relation classification


##SemEval2010_task8

|Models|attention|score|pre-trained|entity position|freeze embed|monitor|batch size| official macro-F1| random search|
|------|---------|-----|-----------|---------------|------------|-------|----------|------------------|--------------|
|entiAttnMatRNN|entity-wise|weight matrix|glove.d100|none|FALSE|val_acc|32| |200|
|attnMatRNN|last hidden|weight matrix|glove.d100|PI|FALSE|val_acc|32| 81.48%|200|
|attnMatRNN|last hidden|weight matrix|glove.d100|none|FALSE|val_acc|32| |200|
|attnRNN(baseline)|all hidden|weight vector|glove.d100|PI|FALSE|val_acc|32| 80.94%|200|

