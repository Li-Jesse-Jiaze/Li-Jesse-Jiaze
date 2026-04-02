
```python
@dataclass
class HumanConfig:
    current_roles: List[Role] = [
        master_student("uni_heidelberg"),
        research_intern("aleph_alpha"),
    ]
    former_roles: List[Role] = [
        algorithm_engineer("qiyuan_lab"),
        bachelor_data_science("tongji_university"),
    ]
    interests: tuple[str, ...] = ("LLMs", "diffusion_models", "3d_vision")


def free_time() -> str:
    return random.choice(["darts", "football", "bird_watching"])
```
