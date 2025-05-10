# CLA

A repository to test cla workflows.


## CLA Assistant

### Initial Notes

1. Grant the app permissions by going through workflow on the [CLA Assistent website[(https://cla-assistant.io/)
2. Create a Gist with the CLA. This can be a "secret" Gist that is not made searchable but is available to anyone with the link.
   1. Gists are version controlled and CLA Assistant managed the process of making people sign up to any new version.
3. Go to the Dashboard on the CLA Assistant website
   1. You may need to refresh the page for it to pick up any newly created repos or Gists.
5. Configure the CLA
   1. Choose a repo
   2. Choose the Gist
   3. Tick "share the Gist" to use one Gist with multiple repos
   4. Leave the options unchanged that trigger a CLA process only once a PR contains a minimum number of changes. IMHO those open us up to poisoned contributions.
6. Once added, people should be able to create PRs on your repo.

### Setup

The following permissions are needed before a CLA can be set up:

<img src="https://github.com/user-attachments/assets/463d7b0a-0ac6-44e5-9042-ebe0052d0fab" width="498"/>

The setup process consists of choosing a repository or organization, a CLA, and the option to "share" the CLA, as well we to not require one for small PRs:

<img width="426" alt="image" src="https://github.com/user-attachments/assets/05a44d45-74e8-4370-811f-1925994bc38b" />

Strangely, on setting up the CLA, CLA Assistant does not show the full set of options. Clicking on the edit button later on reveals more:

<img src="https://github.com/user-attachments/assets/4fe24230-ecf7-4c30-bcb9-8233948fda72" width="597"/>


### Contributor View

Contribtors are prompted to sign the CLA by the CLA Assistant:

<img src="https://github.com/user-attachments/assets/ac42e1cf-28dc-4dea-b0d2-efc82cc6b514" width="905"/>

On clicking on the link to the CLA, they are shown the CLA on the CLA Assistant website and given the option at the bottom to "Sign in with GitHub to agree". The actual process then is the standard Github app authentication workflow:

<img src="https://github.com/user-attachments/assets/35fedd7b-f093-45a8-8585-0887303e7d5f" width="539"/>





### Maintainer View

Maintainers can view the latest signed CLAs on the CLA Assistent website:

![image](https://github.com/user-attachments/assets/2b576c0c-2962-419f-b95c-ee651c085f94)

They can also download the complete history in JSON or CSV. Here is an example JSON download:

```
[
    {
        "user_name": "goatzilla42",
        "gist_name": "individual_cla.md",
        "gist_url": "https://gist.github.com/alexvoss/ff149eab4450354149a9fb092ade0023",
        "gist_version": "4076844bab3cd2eb356ff77e7e63475e43833b29",
        "signed_at": "2025-05-10T13:16:25.753Z",
        "revoked_at": ""
    }
]
```

In the PR, the following appears once all contributors have signed:

<img src="https://github.com/user-attachments/assets/30b7c178-5d17-4294-84ce-9b30a954a921" width="909"/>
