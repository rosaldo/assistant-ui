## aui-perf nightly record

_1 points · 2026-11-18T13:18:13.751Z to 2026-11-18T13:18:13.751Z · latest runner: AMD EPYC 9V74 80-Core Processor · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 702.93µs |  |  | 702.93µs | 702.93µs | 1 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 1.001ms |  |  | 1.001ms | 1.001ms | 1 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 45.21µs |  |  | 45.21µs | 45.21µs | 1 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 522.50µs |  |  | 522.50µs | 522.50µs | 1 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 8.253ms |  |  | 8.253ms | 8.253ms | 1 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 218.58µs |  |  | 218.58µs | 218.58µs | 1 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 2.056ms |  |  | 2.056ms | 2.056ms | 1 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 8.031ms |  |  | 8.031ms | 8.031ms | 1 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 8.34µs |  |  | 8.34µs | 8.34µs | 1 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 69.94µs |  |  | 69.94µs | 69.94µs | 1 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 272.13µs |  |  | 272.13µs | 272.13µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 81.03µs |  |  | 81.03µs | 81.03µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 44.08µs |  |  | 44.08µs | 44.08µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 43.13µs |  |  | 43.13µs | 43.13µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 253.92µs |  |  | 253.92µs | 253.92µs | 1 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 54.14µs |  |  | 54.14µs | 54.14µs | 1 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 525.26µs |  |  | 525.26µs | 525.26µs | 1 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 7.42µs |  |  | 7.42µs | 7.42µs | 1 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 61.93µs |  |  | 61.93µs | 61.93µs | 1 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 591.50µs |  |  | 591.50µs | 591.50µs | 1 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 5.087ms |  |  | 5.087ms | 5.087ms | 1 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 20.015ms |  |  | 20.015ms | 20.015ms | 1 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 289.95µs |  |  | 289.95µs | 289.95µs | 1 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.795ms |  |  | 2.795ms | 2.795ms | 1 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 11.180ms |  |  | 11.180ms | 11.180ms | 1 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 224.73µs |  |  | 224.73µs | 224.73µs | 1 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.683ms |  |  | 1.683ms | 1.683ms | 1 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 50.23µs |  |  | 50.23µs | 50.23µs | 1 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 512.02µs |  |  | 512.02µs | 512.02µs | 1 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.678ms |  |  | 2.678ms | 2.678ms | 1 |
| external-message-conversion › core: external message tool results › 100 matches | 59.84µs |  |  | 59.84µs | 59.84µs | 1 |
| external-message-conversion › core: external message tool results › 1000 matches | 608.75µs |  |  | 608.75µs | 608.75µs | 1 |
| external-message-conversion › core: external message tool results › 5000 matches | 3.166ms |  |  | 3.166ms | 3.166ms | 1 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 31.56µs |  |  | 31.56µs | 31.56µs | 1 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 304.34µs |  |  | 304.34µs | 304.34µs | 1 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.633ms |  |  | 1.633ms | 1.633ms | 1 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.22µs |  |  | 0.22µs | 0.22µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.36µs |  |  | 0.36µs | 0.36µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 2.14µs |  |  | 2.14µs | 2.14µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.49µs |  |  | 0.49µs | 0.49µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.48µs |  |  | 2.48µs | 2.48µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 23.00µs |  |  | 23.00µs | 23.00µs | 1 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 115.00µs |  |  | 115.00µs | 115.00µs | 1 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 594.63µs |  |  | 594.63µs | 594.63µs | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 2.115ms |  |  | 2.115ms | 2.115ms | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 160.41µs |  |  | 160.41µs | 160.41µs | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 2.753ms |  |  | 2.753ms | 2.753ms | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 388.97µs |  |  | 388.97µs | 388.97µs | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 501.03µs |  |  | 501.03µs | 501.03µs | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 5.635ms |  |  | 5.635ms | 5.635ms | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 762.99µs |  |  | 762.99µs | 762.99µs | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 16.387ms |  |  | 16.387ms | 16.387ms | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.738ms |  |  | 2.738ms | 2.738ms | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.933ms |  |  | 1.933ms | 1.933ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 2.322ms |  |  | 2.322ms | 2.322ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.496ms |  |  | 2.496ms | 2.496ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 16.721ms |  |  | 16.721ms | 16.721ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 18.012ms |  |  | 18.012ms | 18.012ms | 1 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.018ms |  |  | 1.018ms | 1.018ms | 1 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 2.161ms |  |  | 2.161ms | 2.161ms | 1 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 7.381ms |  |  | 7.381ms | 7.381ms | 1 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.292ms |  |  | 1.292ms | 1.292ms | 1 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.503ms |  |  | 1.503ms | 1.503ms | 1 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 4.279ms |  |  | 4.279ms | 4.279ms | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 259.09µs |  |  | 259.09µs | 259.09µs | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 2.142ms |  |  | 2.142ms | 2.142ms | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 212.952ms |  |  | 212.952ms | 212.952ms | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 10.572ms |  |  | 10.572ms | 10.572ms | 1 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.83µs |  |  | 1.83µs | 1.83µs | 1 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 9.52µs |  |  | 9.52µs | 9.52µs | 1 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 36.99µs |  |  | 36.99µs | 36.99µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 5.60µs |  |  | 5.60µs | 5.60µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 18.40µs |  |  | 18.40µs | 18.40µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 54.62µs |  |  | 54.62µs | 54.62µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 251.58µs |  |  | 251.58µs | 251.58µs | 1 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 4.692ms |  |  | 4.692ms | 4.692ms | 1 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 33.515ms |  |  | 33.515ms | 33.515ms | 1 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 397.491ms |  |  | 397.491ms | 397.491ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 465.88µs |  |  | 465.88µs | 465.88µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 675.71µs |  |  | 675.71µs | 675.71µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 3.351ms |  |  | 3.351ms | 3.351ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 453.28µs |  |  | 453.28µs | 453.28µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.114ms |  |  | 1.114ms | 1.114ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 14.831ms |  |  | 14.831ms | 14.831ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 459.89µs |  |  | 459.89µs | 459.89µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 842.88µs |  |  | 842.88µs | 842.88µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 8.592ms |  |  | 8.592ms | 8.592ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 219.40µs |  |  | 219.40µs | 219.40µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 410.44µs |  |  | 410.44µs | 410.44µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.779ms |  |  | 2.779ms | 2.779ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 13.86µs |  |  | 13.86µs | 13.86µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 27.27µs |  |  | 27.27µs | 27.27µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 199.22µs |  |  | 199.22µs | 199.22µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 478.66µs |  |  | 478.66µs | 478.66µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 802.07µs |  |  | 802.07µs | 802.07µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 8.706ms |  |  | 8.706ms | 8.706ms | 1 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 202.32µs |  |  | 202.32µs | 202.32µs | 1 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.815ms |  |  | 1.815ms | 1.815ms | 1 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 908.77µs |  |  | 908.77µs | 908.77µs | 1 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 243.84µs |  |  | 243.84µs | 243.84µs | 1 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 2.176ms |  |  | 2.176ms | 2.176ms | 1 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 1.091ms |  |  | 1.091ms | 1.091ms | 1 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 268.05µs |  |  | 268.05µs | 268.05µs | 1 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 20.988ms |  |  | 20.988ms | 20.988ms | 1 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 478.997ms |  |  | 478.997ms | 478.997ms | 1 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 189.84µs |  |  | 189.84µs | 189.84µs | 1 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.573ms |  |  | 1.573ms | 1.573ms | 1 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 806.36µs |  |  | 806.36µs | 806.36µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 166.80µs |  |  | 166.80µs | 166.80µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 779.42µs |  |  | 779.42µs | 779.42µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 182.62µs |  |  | 182.62µs | 182.62µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 821.49µs |  |  | 821.49µs | 821.49µs | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.683ms |  |  | 2.683ms | 2.683ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.705ms |  |  | 2.705ms | 2.705ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.642ms |  |  | 2.642ms | 2.642ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.669ms |  |  | 2.669ms | 2.669ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.695ms |  |  | 1.695ms | 1.695ms | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.534ms |  |  | 2.534ms | 2.534ms | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.543ms |  |  | 2.543ms | 2.543ms | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 204.82µs |  |  | 204.82µs | 204.82µs | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 107.14µs |  |  | 107.14µs | 107.14µs | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.341ms |  |  | 1.341ms | 1.341ms | 1 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.427ms |  |  | 1.427ms | 1.427ms | 1 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.496ms |  |  | 1.496ms | 1.496ms | 1 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 38.46µs |  |  | 38.46µs | 38.46µs | 1 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 40.50µs |  |  | 40.50µs | 40.50µs | 1 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 54.36µs |  |  | 54.36µs | 54.36µs | 1 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.130ms |  |  | 1.130ms | 1.130ms | 1 |

informational; points come from different runners of the same class, so read trends, not single deltas.
