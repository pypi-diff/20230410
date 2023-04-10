# Comparing `tmp/hecto_agent-0.0.2.tar.gz` & `tmp/hecto_agent-0.0.3.tar.gz`

## Comparing `hecto_agent-0.0.2.tar` & `hecto_agent-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 hecto_agent-0.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hecto_agent-0.0.2/ha/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hecto_agent-0.0.2/ha/__init__.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 hecto_agent-0.0.2/ha/beam.py
--rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 hecto_agent-0.0.2/ha/ctc.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 hecto_agent-0.0.2/ha/data.py
--rw-r--r--   0        0        0     9970 2020-02-02 00:00:00.000000 hecto_agent-0.0.2/ha/loop.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 hecto_agent-0.0.2/ha/model.py
--rw-r--r--   0        0        0     8907 2020-02-02 00:00:00.000000 hecto_agent-0.0.2/ha/rnnlm.py
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 hecto_agent-0.0.2/ha/star.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 hecto_agent-0.0.2/ha/symbol_tape.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 hecto_agent-0.0.2/ha/xen.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 hecto_agent-0.0.2/.gitignore
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 hecto_agent-0.0.2/README.md
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 hecto_agent-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 hecto_agent-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/ha/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/ha/__init__.py
+-rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/ha/beam.py
+-rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/ha/ctc.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/ha/data.py
+-rw-r--r--   0        0        0     9970 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/ha/loop.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/ha/model.py
+-rw-r--r--   0        0        0     9059 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/ha/rnnlm.py
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/ha/star.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/ha/symbol_tape.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/ha/transducer.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/ha/xen.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/.gitignore
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/README.md
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 hecto_agent-0.0.3/PKG-INFO
```

### Comparing `hecto_agent-0.0.2/.github/workflows/release.yml` & `hecto_agent-0.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hecto_agent-0.0.2/ha/beam.py` & `hecto_agent-0.0.3/ha/beam.py`

 * *Files identical despite different names*

### Comparing `hecto_agent-0.0.2/ha/ctc.py` & `hecto_agent-0.0.3/ha/ctc.py`

 * *Files identical despite different names*

### Comparing `hecto_agent-0.0.2/ha/data.py` & `hecto_agent-0.0.3/ha/data.py`

 * *Files identical despite different names*

### Comparing `hecto_agent-0.0.2/ha/loop.py` & `hecto_agent-0.0.3/ha/loop.py`

 * *Files identical despite different names*

### Comparing `hecto_agent-0.0.2/ha/model.py` & `hecto_agent-0.0.3/ha/model.py`

 * *Files identical despite different names*

### Comparing `hecto_agent-0.0.2/ha/rnnlm.py` & `hecto_agent-0.0.3/ha/rnnlm.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     def init_hidden(self, batch_size):
         weight = self.out_layer.weight
         h = weight.new_zeros(self.num_layers, batch_size, self.hidden_dim)
         c = weight.new_zeros(self.num_layers, batch_size, self.hidden_dim)
         return (h,c)
 
-    def truncate_hidden(sellf, state):
+    def truncate_hidden(self, state):
         h,c = state
         return (h.detach(), c.detach())
 
 
 
 class System:
     def __init__(self, args):
@@ -70,43 +70,42 @@
                         num_layers=args.num_layers,
                         dropout=args.dropout)
         self.model = self.model.to(args.device)
 
         if args.init:
             self.model.load_state_dict(checkpoint['model'])
 
-        self.optimizer = torch.optim.Adam(params=self.model.parameters(), lr=args.lr)
+        self.optimizer = torch.optim.AdamW(params=self.model.parameters(), lr=args.lr, weight_decay=0.01)
         if args.init:
             self.optimizer.load_state_dict(checkpoint['optimizer'])
 
         self.loss = nn.CrossEntropyLoss(ignore_index=0)
 
         self.log_interval = args.log_interval
-        self.prompts = [
-            "a"
-        ]
+        self.prompts = args.eval_prompts
         self.args = args
 
     def state_dict(self):
         return {
+            'args': vars(self.args),
             'vocab': self.vocab.state_dict(),
             'model': self.model.state_dict(),
             'optimizer': self.optimizer.state_dict()
         }
 
     def prepare_prompt(self, prompt):
         device = next(self.model.parameters()).device
 
         prompt_list = [self.vocab.string_to_id[char] for char in prompt]
         x = torch.tensor(prompt_list).to(device).unsqueeze(1).long()
 
         return x, self.model.init_hidden(1)
 
     @torch.inference_mode()
-    def complete(self, prompt, steps=512, sample=False):
+    def complete(self, prompt, steps=512, top_k=1):
         model = self.model
         model.eval()
 
         joiner = ''
         def cast(s):
             if isinstance(s, int):
                 nonlocal joiner
@@ -115,33 +114,32 @@
             return s
 
         out_list = []
         x, states = self.prepare_prompt(prompt)
 
         logits, states = model(x, states)
         prompt_logits = nn.functional.cross_entropy(logits[:-1], x[1:].view(-1), reduction='none').sum() / len(x[1:])
+
+        v, _ = torch.topk(logits, top_k)
+        logits[logits < v[:, [-1]]] = -float('Inf')
         probs = F.softmax(logits, dim=-1)
         probs = probs[-1]
 
-        if sample:
-            ix = probs.multinomial(num_samples=1)
-        else:
-            max_p, ix = torch.topk(probs, k=1, dim=-1)
+        ix = probs.multinomial(num_samples=1)
 
         out_list.append(cast(self.vocab.id_to_string[int(ix)]))
         x = ix.unsqueeze(1)
 
         # decode
         for k in range(steps):
             logits, states = model(x, states)
+            v, _ = torch.topk(logits, top_k)
+            logits[logits < v[:, [-1]]] = -float('Inf')
             probs = F.softmax(logits, dim=-1)
-            if sample:
-                ix = probs.multinomial(1)
-            else:
-                _, ix = torch.topk(probs, k=1, dim=-1)
+            ix = probs.multinomial(num_samples=1)
             out_list.append(cast(self.vocab.id_to_string[int(ix)]))
             x = ix
         return prompt_logits, joiner.join(out_list)
 
     def train_one_epoch(self, epoch=0):
         model, batches = self.model, self.batches
         optimizer, loss_fn = self.optimizer, self.loss
@@ -166,26 +164,24 @@
             output, state = model(input, state)
             loss = loss_fn(output, target)
             loss.backward()
             grad_norm = torch.nn.utils.clip_grad_norm_(model.parameters(), 1)
             optimizer.step()
 
             if step % self.log_interval == 0:
-                print(f"epoch {epoch} step {step}/{len(batches)} train loss: {loss.item():.3f} ppl: {loss.exp().item():.3f} grad_norm: {grad_norm.item():.3f}")
-                for prompt in self.prompts:
-                    _, generated_text = self.complete(prompt, 128, sample=False)
-                    print('greedy', prompt + generated_text)
+                outputs = []
                 for prompt in self.prompts:
-                    _, generated_text = self.complete(prompt, 128, sample=True)
-                    print('sample', prompt + generated_text)
+                    _, generated_text = self.complete(prompt, 128, top_k=self.args.top_k)
+                    outputs.append(prompt + generated_text)
+                print(f"epoch {epoch} step {step}/{len(batches)} loss: {loss.item():.3f} ppl: {loss.exp().item():.3f} grad_norm: {grad_norm.item():.3f} {'; '.join(outputs)}")
                 wandb.log({'train/loss': loss.item(),
-                          'train/ppl': loss.exp().item(),
-                          'train/lr': self.args.lr,
-                          'train/epoch': epoch,
-                          'train/grad_norm': grad_norm.item()})
+                           'train/ppl': loss.exp().item(),
+                           'train/lr': self.args.lr,
+                           'train/epoch': epoch,
+                           'train/grad_norm': grad_norm.item()})
             else:
                 wandb.log({'train/loss': loss.item(),
                            'train/ppl': loss.exp().item(),
                            #'train/lr': scheduler.get_last_lr()[0],
                            'train/lr': self.args.lr,
                            'train/epoch': epoch,
                            'train/grad_norm': grad_norm.item()})
@@ -206,36 +202,36 @@
     parser.add_argument('--batch-size', default=128, type=int, help='batch size')
     parser.add_argument('--bptt-len', default=256, type=int, help='RNN window size')
     parser.add_argument('--rnn-size', default=512, type=int, help='RNN width')
     parser.add_argument('--num-layers', default=1, type=int, help='RNN depth')
     parser.add_argument('--bytes-as-tokens', action='store_true', help='use bytes as tokens')
     parser.add_argument('--train', type=Path, help='Train model on this data')
     parser.add_argument('--complete', type=str, help='complete this prompt')
+    parser.add_argument('--top-k', type=int, default=1, help='top-k sampling')
     parser.add_argument('--log-interval', type=int, default=100, help="Number of batches between printing training status")
+    parser.add_argument('--eval-prompts', type=str, nargs='+', default=['\nа', '\nя'], help="Prompts to complete during evaluation")
     args = parser.parse_args()
 
     if not args.train and not args.complete:
         parser.print_help()
-        print("\nPlease specify either --train or --init", file=sys.stderr)
+        print("\nPlease specify either --train or --complete", file=sys.stderr)
         sys.exit(1)
 
-    print(args)
-
     torch.manual_seed(3407)
 
     self = System(args)
 
     if args.train:
+        print(args)
         wandb.init(project='rnnlm', config=args)
 
         for epoch in range(args.epochs):
             self.train_one_epoch(epoch=epoch)
             torch.save(self.state_dict(), args.save)
 
     if args.complete:
         self.model.eval()
-        prompt_score, completion = self.complete("\n" + args.complete, 128, sample=False)
+        prompt_score, completion = self.complete("\n" + args.complete, 1024, top_k=args.top_k)
         print(prompt_score.item(), args.complete + completion)
 
-
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hecto_agent-0.0.2/ha/star.py` & `hecto_agent-0.0.3/ha/star.py`

 * *Files identical despite different names*

### Comparing `hecto_agent-0.0.2/ha/symbol_tape.py` & `hecto_agent-0.0.3/ha/symbol_tape.py`

 * *Files identical despite different names*

### Comparing `hecto_agent-0.0.2/ha/xen.py` & `hecto_agent-0.0.3/ha/xen.py`

 * *Files identical despite different names*

### Comparing `hecto_agent-0.0.2/pyproject.toml` & `hecto_agent-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hecto_agent-0.0.2/PKG-INFO` & `hecto_agent-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hecto-agent
-Version: 0.0.2
+Version: 0.0.3
 Summary: hecto speech agent for 100 hours
 Project-URL: Documentation, https://github.com/proger/ha1#readme
 Project-URL: Issues, https://github.com/proger/ha1/issues
 Project-URL: Source, https://github.com/proger/ha1
 Author-email: Volodymyr Kyrylov <vol@wilab.org.ua>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

