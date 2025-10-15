
```python
@dataclass
class HumanConfig:
    current_roles: List[Role] = [
        m_sc_student("uni_heidelberg"),
        working_student("aleph_alpha"),
    ]
    former_roles: List[Role] = [
        algorithm_engineer("qiyuan_lab"),
        b_eng_data_science("tongji_university"),
    ]
    interests: tuple[str, ...] = ("LLMs", "diffusion_models", "vision_3d")


def free_time() -> str:
    return random.choice(["darts", "football", "bird_watching"])
```
