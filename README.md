# ClassModel_torch_nn_Module(模型學習與理解)

導入了必要的庫，包括torch、torch.nn和torchviz。

定義了一個名為Model的簡單的PyTorch模型，該模型具有三個線性層（神經網絡層），用於示範模型的結構。

創建了一個Model的實例，並指定了輸入特徵的維度和輸出特徵的維度。

創建了一個虛擬的輸入tensor dummy_input，該tensor的形狀是(1, input_size)，這是因為模型需要接受一個形狀為(batch_size, input_size)的輸入。

使用make_dot函數可視化模型的計算圖。model(dummy_input)表示將虛擬輸入dummy_input通過模型前向傳播，然後params=dict(model.named_parameters())用於傳遞模型的參數信息，以便可視化模型的結構。
