# attention-based relation classification


##SemEval2010_task8

|Models|attention|score|pre-trained|position feats|monitor|batch size| official macro-F1|checkpoint|random search| speed|
|------|---------|-----|-----------|---------------|-------|----------|------------------|----------|--------------|-----|
|entiAttnMatRNN|entity-wise|weight matrix|glove.d100|none|val_acc|32| 81.43% |epoch|200|11s/epoch|
|entiAttnMatRNN|entity-wise|weight matrix|glove.d100|none|val_acc|32| 82.70% |step|1|210s/epoch|
|attnMatRNN|last hidden|weight matrix|glove.d100|PI|val_acc|32| 80.93%|epoch|200|
|attnMatRNN|last hidden|weight matrix|glove.d100|none|val_acc|32| 68.83%|epoch|200|
|attnRNN(baseline)|all hidden|weight vector|glove.d100|PI|val_acc|32| 80.59%|epoch|200|3s/epoch|
|attnRNN(baseline)|all hidden|weight vector|glove.d100|PI|val_acc|32| 82.49%(84.0%)|step|1|10s/epoch|
|attnRNN(baseline)|all hidden|weight vector|glove.d100|none|val_acc|32|70.90%|epoch|200|3s/epoch|
||||||||||||
|entiAttnMatRNN|entity-wise|weight matrix|glove.d100|none|val_acc|32| 83.26% |10steps|200|30s/epoch|
|attnRNN(baseline)|all hidden|weight vector|glove.d100|PI|val_acc|32|82.97%|10steps|200|12s/epoch|
|RNN(baseline)|none|none|glove.d100|PI|val_acc|32| 81.87% |10steps|200|9s/epoch|

Runing:
1) input attention

TO-DO:
1) improve the speed of indexing entity tokens from sequence (2s/epoch -> 11s/epoch)
2) macro-f1(excluding 'Other') monitor
