it's part of the project meta's capstone

testable urls

urlpatterns = [
    path("", views.index, name="index"),
    path("menu/", views.MenuItemsView.as_view()),
    path("menu/<int:pk>", views.SingleMenuItemView.as_view()),
    path("", include(router.urls)),
    path("api-token-auth/", obtain_auth_token),
]
