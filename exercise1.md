# exercise 1

## CI setup on Rust

Rust is mostly unfamiliar to me so let's see what it has to offer.

### Linting

The most common answer for linting in Rust seems to be clippy. As for code formatting there is rustfmt.

### Testing

The most obvious choice for testing is Rust's own package manager's cargo test. Apparently there is a
newer tester that is said to be faster and with more features cargo nextest.

### Building

Once again rust has has a obvious solution for this and it's cargo build.

## Alternatives to Jenkins and GitHub Actions?

Close alternative to GitHub Actions is GitLab's own CI/CD setup which also uses yml files for configuring your environment.
Cloud-hosting platforms offer their own setups like Azure pipeline and AWS CodePipeline.
CircleCI is an other popular choice and companies like Spotify and Sony has used it.
For enterprises there is TeamCity from JetBrains that can be both cloud- and self-hosted.

## Self-hosted or a cloud-based env?

If the applications is made by 6 people, the scope of the app is probably not large enough where we would need
to self-host our own environment. Especially if we want to release the application soon, setting up GitHub Actions
is way faster than configuring our own setup. That is if our requirements for CI is fairly "vanilla" and doesn't require
specialized environment. Later on if the scope of the app grows we could look into self-hosting.
