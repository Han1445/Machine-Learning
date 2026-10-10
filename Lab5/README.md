Task 1: I added a delivery\_fee\_ratio feature (delivery fee divided by the total order) because people are way more likely to cancel if the delivery charge takes up a huge chunk of their bill.



Task 2: For is\_peak\_hour, I tested narrowing it down strictly to the evening dinner rush (17:00 to 22:00) instead of both lunch and dinner. The overall accuracy stayed pretty close, but it really helped the model focus better on those crazy dinner cancellations.



Task 3: I played around with top\_k grouping for messy categorical features like delivery areas ($k$ at 10, 20, and 40). Keeping it at a smaller $k$ like 10 stopped it from overfitting, while cranking it up just made things too noisy.



Task 4: I ran SelectFromModel to drop unneeded features. Since the dataset is super imbalanced, it didn't magically fix my accuracy score, but it definitely cleaned up the model and made training a lot faster by cutting out the dead weight.

