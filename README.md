
```python
@dataclass(frozen=True)
class Role:
    title: str
    org: str
    current: bool = True


@dataclass(frozen=True)
class HumanConfig:
    roles: tuple[Role, ...] = (
        Role("MSc Student", "Uni Heidelberg"),
        Role("Research Intern", "Aleph Alpha"),
        Role("Algorithm Engineer", "Qiyuan Lab", current=False),
        Role("BSc Data Science", "Tongji University", current=False),
    )
    interests: tuple[str, ...] = ("LLMs", "diffusion_models", "3d_vision")
```
