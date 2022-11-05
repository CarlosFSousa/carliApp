<script>
  import { Link } from 'svelte-navigator';
</script>

<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container-fluid">
    <Link class="navbar-brand" to="/">C&A</Link>
    <button
      class="navbar-toggler"
      type="button"
      data-bs-toggle="collapse"
      data-bs-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon" />
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <Link class="nav-link" aria-current="page" to="/whereandwhen"
            >Where & When</Link
          >
        </li>
        <li class="nav-item">
          <Link class="nav-link" to="/expectations">What to expect</Link>
        </li>
        <li class="nav-item">
          <Link class="nav-link" to="/tips">Tips</Link>
        </li>
        <li class="nav-item">
          <Link class="nav-link" to="/azores">Azores</Link>
        </li>
      </ul>
      <button type="submit" class="me-2 btn btn-secondary"
        >Confirm your presence</button
      >
    </div>
  </div>
</nav>
