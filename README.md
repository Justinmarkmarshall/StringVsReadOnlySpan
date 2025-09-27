# StringVsReadOnlySpan

| Method                | Job        | Toolchain              | N    | Mean          | Error         | StdDev        | Ratio | RatioSD | Gen0    | Gen1   | Allocated | Alloc Ratio |
|---------------------- |----------- |----------------------- |----- |--------------:|--------------:|--------------:|------:|--------:|--------:|-------:|----------:|------------:|
| Contains_String       | Job-IHMLWV | InProcessEmitToolchain | 64   |     13.724 ns |     0.7646 ns |     0.7152 ns |  1.00 |    0.00 |       - |      - |         - |          NA |
| Contains_ReadOnlySpan | Job-IHMLWV | InProcessEmitToolchain | 64   |      9.074 ns |     0.4835 ns |     0.4523 ns |  0.66 |    0.05 |       - |      - |         - |          NA |
| Trim_String           | Job-IHMLWV | InProcessEmitToolchain | 64   |     46.207 ns |    10.8351 ns |    10.1352 ns |  3.35 |    0.65 |  0.0242 |      - |     152 B |          NA |
| Trim_ReadOnlySpan     | Job-IHMLWV | InProcessEmitToolchain | 64   |     24.185 ns |     5.6928 ns |     5.3250 ns |  1.78 |    0.45 |       - |      - |         - |          NA |
| CountCsv_StringSplit  | Job-IHMLWV | InProcessEmitToolchain | 64   |    230.605 ns |    14.7281 ns |    13.0561 ns | 16.94 |    1.11 |  0.1056 | 0.0002 |     664 B |          NA |
| CountCsv_ReadOnlySpan | Job-IHMLWV | InProcessEmitToolchain | 64   |    134.897 ns |     7.3136 ns |     6.4833 ns |  9.90 |    0.40 |       - |      - |         - |          NA |
| TryParse_Int_String   | Job-IHMLWV | InProcessEmitToolchain | 64   |     14.953 ns |     0.9764 ns |     0.8153 ns |  1.10 |    0.07 |       - |      - |         - |          NA |
| TryParse_Int_Span     | Job-IHMLWV | InProcessEmitToolchain | 64   |     14.157 ns |     0.7483 ns |     0.7000 ns |  1.03 |    0.08 |       - |      - |         - |          NA |
