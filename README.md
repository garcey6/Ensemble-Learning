# Ensemble-Learning
掌握应用投票方法进行类别预测的方法。 理解bagging，boosting和stacking三类集成方法，掌握随机森林、adaboost和梯度提升学习算法。


练习题
1. 加载Fashion-MNIST数据集，将其分为一个训练集、一个验证集和一个测试集（例如使用40000个实例训练，10000个实例验证，最后10000个实例测试）。然后训练多个分类
器，比如一个随机森林分类器、一个极端随机树分类器和一个SVM。接下来，尝试使用软投票法或
者硬投票法将它们组合成一个集成，这个集成在验证集上的表现要胜过它们各自单独的表现。成功
找到集成后，在测试集上测试。与单个的分类器相比，它的性能要好多少？
2. 运行上一个练习中的单个分类器，用验证集进行预测，然后用预测结果创建一个新的训练集：新训
练集中的每个实例都是一个向量，这个向量包含所有分类器对于一张图像的一组预测，目标值是图
像的类别。恭喜，你成功训练了一个混合器，结合第一层的分类器，它们一起构成了一个stacking
集成。现在在测试集上评估这个集成。对于测试集中的每张图像，使用所有的分类器进行预测，然
后将预测结果提供给混合器，得到集成的预测。与前面训练的投票分类器相比，这个集成的结果如何？
