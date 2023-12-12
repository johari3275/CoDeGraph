# MC CoDe-Graph Improvement Ideas

Suggestion for improvement:
- Scaffolding as an element (e.g., moderator, prompt…)
- Badge element for finishing the course.
- Connecting arrows forward and backward (if student can move back as well; e.g, rewatching an instructional video)
- Locked and unlocked affordances symbols
- Assessment and feedback elements should be kept separately and connected with a line.
- Sequencing should be obvious to the viewer of a design.

### Design 1: MC CoDe-Graph traditional design (based on current model)
[![](https://mermaid.ink/img/pako:eNrVlV1v2jAYhf-K5d5QiaCEEAhZhcTHwrbChtRqFxAuTPIGrCZ2ZDtdGep_n_PRri1j1bTe9A7lnPf4PHGMDzjkEWAPxwn_Ee6IUOh6ErCAhQmRcgIx4oKwLaCYJol3FsfEMc0PT-Q9JHryUY7j53JG2U0t-v7YHI-0KNU-AbSsHqOzDXGcyC7WHK5WPmUkQdcg1XrteV69uGEYaDkY81xIQGOeZgkoyhm62IgBGpFoC-tifrRazW0PLQQYf0oYDRsNHyDakPDm_FxrZTmjNQMiGAgUE5pIlOlppaer8JTfgkSKo6QwUbZFtzQC3jIGaNwoV5s9CN8LYV3k1u_kwtCuSeW6UpBJ3YyHIOWR6WMdRWPY6XLHBr8kW3CpXpIV3FOttv_CPX1T7k-NcrVXuD9XLl9_CLuQiOiY6UvluAqBEUGPEy5LqlPMs8bc-o18_oJ49qbEc93UepX4a-Wa54miimyO9G91yslNXqxKwyni0ewJgczDUANKRNkpDgZ36lErMKY6Y_qfGSOdMfy3DH3OizP9kDAM2OJUQEH-WotKe76Tx7NS5RHV04-bmRIFghJtJltC678OohSkmZJPpis1Z4omVTcp63d3-f5a693y319r_YXgJk5BpIRG-mo6BAyhAKsdpBBgT_-MICb6mAU4YPfaSnLFr_YsxJ4SOTRxnkW6wYSSrSAp9mLdRD-FiCou5tV1V956TZwRhr0DvsOe63Rb_Xbfsbtuz7Stdq-J99gzrI7bafWsdrfXdkzb7vfvm_gn5zq10zJdt911-rbpWlbHcsu0ZamVK97_AvO0dLM?type=png)](https://mermaid.live/edit#pako:eNrVlV1v2jAYhf-K5d5QiaCEEAhZhcTHwrbChtRqFxAuTPIGrCZ2ZDtdGep_n_PRri1j1bTe9A7lnPf4PHGMDzjkEWAPxwn_Ee6IUOh6ErCAhQmRcgIx4oKwLaCYJol3FsfEMc0PT-Q9JHryUY7j53JG2U0t-v7YHI-0KNU-AbSsHqOzDXGcyC7WHK5WPmUkQdcg1XrteV69uGEYaDkY81xIQGOeZgkoyhm62IgBGpFoC-tifrRazW0PLQQYf0oYDRsNHyDakPDm_FxrZTmjNQMiGAgUE5pIlOlppaer8JTfgkSKo6QwUbZFtzQC3jIGaNwoV5s9CN8LYV3k1u_kwtCuSeW6UpBJ3YyHIOWR6WMdRWPY6XLHBr8kW3CpXpIV3FOttv_CPX1T7k-NcrVXuD9XLl9_CLuQiOiY6UvluAqBEUGPEy5LqlPMs8bc-o18_oJ49qbEc93UepX4a-Wa54miimyO9G91yslNXqxKwyni0ewJgczDUANKRNkpDgZ36lErMKY6Y_qfGSOdMfy3DH3OizP9kDAM2OJUQEH-WotKe76Tx7NS5RHV04-bmRIFghJtJltC678OohSkmZJPpis1Z4omVTcp63d3-f5a693y319r_YXgJk5BpIRG-mo6BAyhAKsdpBBgT_-MICb6mAU4YPfaSnLFr_YsxJ4SOTRxnkW6wYSSrSAp9mLdRD-FiCou5tV1V956TZwRhr0DvsOe63Rb_Xbfsbtuz7Stdq-J99gzrI7bafWsdrfXdkzb7vfvm_gn5zq10zJdt911-rbpWlbHcsu0ZamVK97_AvO0dLM)


Description:
- Badge element included
- Connecting arrows forward and backward included for learning materials (M1 – M3)
- Locked and unlocked affordances symbols visualized by outer layer of building block (e.g., M2-pretest or M3-post-test)
- Assessment and Feedback connected via line
- Sequencing obvious based on flow from left to right

Mermaid Syntaxt for Design 1:
```
flowchart TD

classDef orange fill:#ffa500
classDef yellow fill:#ffff00
classDef pink fill:#FFC0CB
classDef green fill: #00ff00
classDef turquoise fill: #4FF2E7
classDef purple fill: #ba55d3

A[[Final Test <br>Essay]]:::green --- Z>Course Completion <br> Badge]:::purple

B[[M3: Pre-Test]]:::orange --- BA((Feedback)):::pink -.Learner fails pre-test <br> moves to learning video.-> C([M3: Learning Video]):::yellow <--> CA([Scaffolding: <br> ChatBot Intervention]):::turquoise <--> D([M3: Steps Process]):::yellow <--> E([M3: Lifehacks]):::yellow <--> F[[M3:Post-Test]]:::orange

G[[M2: Pre-Test]]:::orange --- BG((Feedback)):::pink -.Learner fails pre-test <br> moves to learning video.-> H([M2: Learning Video]):::yellow <--> HA([Scaffolding: <br> Prompt with Tips]):::turquoise <--> I([M2: Flashcards]):::yellow <--> J([M2: Scenario]):::yellow <--> K[[M2:Post-Test]]:::orange

L(M1: Pre-Test):::orange --- BL((Feedback)):::pink -.Learner fails pre-test <br> moves to learning video.-> M([M1: Learning Video]):::yellow  <--> MA([Scaffolding: <br> Q&A with Moderator]):::turquoise <--> N([M1: Multitab]):::yellow <--> O([M1: Lifehacks]):::yellow <--> P[[M1: Post-Test]]:::orange

BL -.Learner succeeds in pre-test <br> moves to next pre-test.-> G
BG -.Learner succeeds in pre-test <br> moves to next pre-test.-> B
BA -.Learner succeeds in pre-test <br> moves to  final test.-> A
P -.Learner succeeds in post-test <br> moves to next pre-test <br> Learner fails in post-test <br> studies learning materials again <br> attempts post-test again until success.-> G
K -.Learner succeeds in post-test <br> moves to next pre-test <br> Learner fails in post-test <br> studies learning materials again <br> attempts post-test again until success.-> B
F -.Learner succeeds in post-test <br> moves to next pre-test <br> Learner fails in post-test <br> studies learning materials again <br> attempts post-test again until success.-> A

```

### Design 2: MC CoDe-Graph traditional design + Scaffolding block + ELO block
[![](https://mermaid.ink/img/pako:eNrVll1v2jAUhv-K5UkTlQhK-CaqKvHRtF1hY6LaRUkvTOKA1cTObKctq_rfd5wApQVaTetN7xDvOe95_eCc8IgDEVLs4igW98GCSI2uBj73eRATpQY0QkISPqcoYnHsfoki0rDtLXVJY2jcqFH0Qk0Zv11pnte3-70tbS4p5YWIvtj2q06dyd-ZYIquK-qeVz1tbXtnMo038ow0GmHNBO9Opx7jJEZXVGl0PJMnp0qR5c2N67rFTMuy0PVJX2QS7PsiARvNBM9rUY-Ec2pqC3_j2JtORzUXjSW1jGfutKJirHrdUsmjNJyR4PboyHSaU1uVISWSU4kiwmKFUujW60QoEXdUIS1QbIoYn6M7FlJRsU5Qv5RPG66FX0a4Mb4r1seWqeqWppOARJGIQ6hyC9v-guie0OiCayrvKDfHylufcebdg2LGRNNUwblEQJXaGXG6CsIiuoCj7RZ4OZexUPo1F0PtDNTqG9TOPpTaeSmf9g61873UAECSanTP9AJdsVTtI3ZR-Htw-xYBkeEujW9FxSSgnEi2O_sy53GI1rA0cp5hHb1iNfxQViNI6rzFqgg82gvr59duQWoEe0MSLeQ-XN-LEaMs1kyT2Q6MH6sIB-_WeJoXHMLVG24dX2VBAHQUYvwQBE4f9EYzDM7A4-w_PWCb9br_5gHryqymtUPX5-NDBubk76UotJfXYLdX6Sxk0L25CQmB9cAIFJM5YavFR7Sm8Biore5CzWCNxEU2pVbsLj9favi1vM-XGm4ILuOEyoSwEF7Tjz5HyMd6QRPqYxc-hjQi8Jj52OdPUEoyLSZLHmBXy4yWcZaGkGDAyFySBLsRJIFvacjgyR0Vr_78H0AZp4Rj9xE_YLfdaFY61U6j1my37JpTbZXxEruWU2_XKy2n2mxVG3at1uk8lfEfIcC1XrHb7Wqz0anZbcepO-3c7TrX8olPfwF2Zs_U?type=png)](https://mermaid.live/edit#pako:eNrVll1v2jAUhv-K5UkTlQhK-CaqKvHRtF1hY6LaRUkvTOKA1cTObKctq_rfd5wApQVaTetN7xDvOe95_eCc8IgDEVLs4igW98GCSI2uBj73eRATpQY0QkISPqcoYnHsfoki0rDtLXVJY2jcqFH0Qk0Zv11pnte3-70tbS4p5YWIvtj2q06dyd-ZYIquK-qeVz1tbXtnMo038ow0GmHNBO9Opx7jJEZXVGl0PJMnp0qR5c2N67rFTMuy0PVJX2QS7PsiARvNBM9rUY-Ec2pqC3_j2JtORzUXjSW1jGfutKJirHrdUsmjNJyR4PboyHSaU1uVISWSU4kiwmKFUujW60QoEXdUIS1QbIoYn6M7FlJRsU5Qv5RPG66FX0a4Mb4r1seWqeqWppOARJGIQ6hyC9v-guie0OiCayrvKDfHylufcebdg2LGRNNUwblEQJXaGXG6CsIiuoCj7RZ4OZexUPo1F0PtDNTqG9TOPpTaeSmf9g61873UAECSanTP9AJdsVTtI3ZR-Htw-xYBkeEujW9FxSSgnEi2O_sy53GI1rA0cp5hHb1iNfxQViNI6rzFqgg82gvr59duQWoEe0MSLeQ-XN-LEaMs1kyT2Q6MH6sIB-_WeJoXHMLVG24dX2VBAHQUYvwQBE4f9EYzDM7A4-w_PWCb9br_5gHryqymtUPX5-NDBubk76UotJfXYLdX6Sxk0L25CQmB9cAIFJM5YavFR7Sm8Biore5CzWCNxEU2pVbsLj9favi1vM-XGm4ILuOEyoSwEF7Tjz5HyMd6QRPqYxc-hjQi8Jj52OdPUEoyLSZLHmBXy4yWcZaGkGDAyFySBLsRJIFvacjgyR0Vr_78H0AZp4Rj9xE_YLfdaFY61U6j1my37JpTbZXxEruWU2_XKy2n2mxVG3at1uk8lfEfIcC1XrHb7Wqz0anZbcepO-3c7TrX8olPfwF2Zs_U)


Description:
- Study Coordination course as a template
- Scaffolding blocks included with example text
- ELO block included (Essay replaced the final test)

Mermaid Syntaxt for Design 2:
```
flowchart TD

classDef orange fill:#ffa500
classDef yellow fill:#ffff00
classDef pink fill:#FFC0CB
classDef green fill: #00ff00
classDef turquoise fill: #4FF2E7
classDef purple fill: #ba55d3

A[[Final Test <br>Essay]]:::green --- Z>Course Completion <br> Badge]:::purple

B[[M3: Pre-Test]]:::orange --- BA((Feedback)):::pink -.Learner fails pre-test <br> moves to learning video.-> C([M3: Learning Video]):::yellow <--> CA([Scaffolding: <br> ChatBot Intervention]):::turquoise <--> D([M3: Steps Process]):::yellow <--> E([M3: Lifehacks]):::yellow <--> F[[M3:Post-Test]]:::orange

G[[M2: Pre-Test]]:::orange --- BG((Feedback)):::pink -.Learner fails pre-test <br> moves to learning video.-> H([M2: Learning Video]):::yellow <--> HA([Scaffolding: <br> Prompt with Tips]):::turquoise <--> I([M2: Flashcards]):::yellow <--> J([M2: Scenario]):::yellow <--> K[[M2:Post-Test]]:::orange

L(M1: Pre-Test):::orange --- BL((Feedback)):::pink -.Learner fails pre-test <br> moves to learning video.-> M([M1: Learning Video]):::yellow  <--> MA([Scaffolding: <br> Q&A with Moderator]):::turquoise <--> N([M1: Multitab]):::yellow <--> O([M1: Lifehacks]):::yellow <--> P[[M1: Post-Test]]:::orange

BL -.Learner succeeds in pre-test <br> moves to next pre-test.-> G
BG -.Learner succeeds in pre-test <br> moves to next pre-test.-> B
BA -.Learner succeeds in pre-test <br> moves to  final test.-> A
P -.Learner succeeds in post-test <br> moves to next pre-test <br> Learner fails in post-test <br> studies learning materials again <br> attempts post-test again until success.-> G
K -.Learner succeeds in post-test <br> moves to next pre-test <br> Learner fails in post-test <br> studies learning materials again <br> attempts post-test again until success.-> B
F -.Learner succeeds in post-test <br> moves to next pre-test <br> Learner fails in post-test <br> studies learning materials again <br> attempts post-test again until success.-> A

```
### Design 3: MC CoDe-Graph BPMN 2.0 oriented
[![](https://mermaid.ink/img/pako:eNrVVV1v2jAU_SuWK01BIigQwkdUVeKjoVvJxkS1hzZ9MIkDVhM7s522DPHfZydAKYVN0_rSN_C599xzj2-uVzBkEYYujBP2FC4Ql-BmGNCAhgkSYohjwDiicwxikiTuWRwjx7L20CVOVOIOjeNXaEbowwbzvIE16O9hc44xLUFwZlkHmTLnP3NGBN5GND2vcdne5855luzgGXKcyK4KydkDds9s266C8o_5RCK5cIGTPeu-eoZHKErADRYSnM_4xaUQaFlxXbcUZJomuDWMAcu5Kj5gqSoiCaNFLOijaI4rOrosrxn7hm-7YMKxqTk1trFMU_V7Kw_jaIbCh7XO0oaYtTFGnGIOYkQSATKVKrdyQMoesQCSgUQHEToHjyTCrGZegMGdrjTenv_Q5_eKdXMJ56aO6RnTEMUxSyIV45acgwWSfSbBZyoxf8RUN6SFvrhc5A6LTqYSZ0L1w0IsROWA_rIIGZMYL1RLb2BPwxMm5IEX2qfR3Z3feDHq_v7AqdE7OnVVlPqzU1fHnFJtp5kET0QuwA3JxBGXPhua21NzuAgRj9548KXApyGmiBN2iF5r9IRDY8Mw_PreLFUOp2n8jh75Ra3XHu2pLeX6x0z6_qlXOuSr3cGRZPyITV8Lej9PJJFodmjDt7L4qTmalD4ct6k_3mta5GGoLBGA0FOtU_wsd5jufKQ4Rv_JoVZZv_dvHGpX6c2zZegFdHKKQDf-NxUl9vry3-YKmUdEZe_uP0VqBxCkgtEckc1eQ1JiNfdiL7tEc7UrklKbEBvvrj-eanVb3sdTrSYEVmGKeYpIpN7oVUABCKBc4BQH0FU_Ixwj9YUFMKBrFYpyyaZLGkJX8hxXYZ5FSsGQoDlHKXRjpUSd4oioT9Yv3_3i-a_CDFHoruAzdDtOq9ZtdB271Wlbdr3RrsIldM16s9OsteuNVrvhWLbd7a6r8BdjirVZszqdRsvp2lanXm_WOwXbbYEVFde_AahiznQ?type=png)](https://mermaid.live/edit#pako:eNrVVV1v2jAU_SuWK01BIigQwkdUVeKjoVvJxkS1hzZ9MIkDVhM7s522DPHfZydAKYVN0_rSN_C599xzj2-uVzBkEYYujBP2FC4Ql-BmGNCAhgkSYohjwDiicwxikiTuWRwjx7L20CVOVOIOjeNXaEbowwbzvIE16O9hc44xLUFwZlkHmTLnP3NGBN5GND2vcdne5855luzgGXKcyK4KydkDds9s266C8o_5RCK5cIGTPeu-eoZHKErADRYSnM_4xaUQaFlxXbcUZJomuDWMAcu5Kj5gqSoiCaNFLOijaI4rOrosrxn7hm-7YMKxqTk1trFMU_V7Kw_jaIbCh7XO0oaYtTFGnGIOYkQSATKVKrdyQMoesQCSgUQHEToHjyTCrGZegMGdrjTenv_Q5_eKdXMJ56aO6RnTEMUxSyIV45acgwWSfSbBZyoxf8RUN6SFvrhc5A6LTqYSZ0L1w0IsROWA_rIIGZMYL1RLb2BPwxMm5IEX2qfR3Z3feDHq_v7AqdE7OnVVlPqzU1fHnFJtp5kET0QuwA3JxBGXPhua21NzuAgRj9548KXApyGmiBN2iF5r9IRDY8Mw_PreLFUOp2n8jh75Ra3XHu2pLeX6x0z6_qlXOuSr3cGRZPyITV8Lej9PJJFodmjDt7L4qTmalD4ct6k_3mta5GGoLBGA0FOtU_wsd5jufKQ4Rv_JoVZZv_dvHGpX6c2zZegFdHKKQDf-NxUl9vry3-YKmUdEZe_uP0VqBxCkgtEckc1eQ1JiNfdiL7tEc7UrklKbEBvvrj-eanVb3sdTrSYEVmGKeYpIpN7oVUABCKBc4BQH0FU_Ixwj9YUFMKBrFYpyyaZLGkJX8hxXYZ5FSsGQoDlHKXRjpUSd4oioT9Yv3_3i-a_CDFHoruAzdDtOq9ZtdB271Wlbdr3RrsIldM16s9OsteuNVrvhWLbd7a6r8BdjirVZszqdRsvp2lanXm_WOwXbbYEVFde_AahiznQ)


- Shapes of objects oriented at BPMN 2.0
- Therefore, shape of elements based on the positioning and purpose in the flowchart instead of base shape (e.g., CoDe-Graph building blocks are always the same shape)
- Shape of objects identical besides:
  - Starting point: circle with a thin outer layer
  - Gateway (Branching): rhombus-shaped object (for feedback in this case)
  - End point: circle with thick outer layer


### Viewing the mermaid syntax

Option 1:
- Copy the above syntax
- Go to https://mermaid.live
- Paste in the code section and the diagram will be automatically generated (if there is no syntax error)

![image](https://github.com/johari3275/CoDeGraph/assets/111693027/a8d3fedc-d265-4108-9575-b06a9f5ecd09)

Option 2:
- Copy the above syntax
- Go to https://draw.io
- Go to Arrange option -> Insert -> Advanced -> mermaid

![image](https://github.com/johari3275/CoDeGraph/assets/111693027/c327e275-ddfe-4ad6-9234-2263e671bdc0)

